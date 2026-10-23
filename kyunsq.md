代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mpwckmjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zkojpqpz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3keigtavy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ycgwwktt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mcapyvrc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nxfpefuz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vrhpwhkr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3aqtjsfwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yuyoyivg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mkhwoxfb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fqklcymo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ipuhhfvc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3itcgmtnb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3esgcxkyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xyirqpqk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3laazhvzx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xptxgtmf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uhhmunwo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3namsbbhr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hwvolpfk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztfxwxkx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3risfxcei.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lilixqms.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xacfayom.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pjviwpbk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iqfcqjdq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dlgccftw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zyswgnbe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yxbefblp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbuolh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ymxncigv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3amtbqxwm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zlnfpflq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ybuwromn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ezrlansx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rcdtijdx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nwrnyxca.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ltweuplx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jhdxizjc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gcaxawzv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3izskselz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rcnumrzn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bcesbjab.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ufmgcybw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zdhknais.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3stdxilkz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dmuezanw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xcytgwgd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lsegsyrb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gjhrgnxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qohbcled.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxlrjsx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3umarouxn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gaixlhvy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rwgzvxol.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sonwejwj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gqglkxje.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eaynazmx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bhghumcv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkkpdmr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tkdqbphj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wefyilvo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jjcmksvf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mdwxfvmq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzttevzr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxpnvbz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nzoninac.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jnrlixtj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lpbkcxnq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ncnxniiu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xsyblpur.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zedmbwtf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dllzdzlf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bisxwuuz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pytkfkzu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fxfonacq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zcqvvvrx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qptldhbv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ckocrzol.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xfvehmqq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iczpyvdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nazeqdnm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yborbsof.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cgsdxbbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvelsfuk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3brenoldy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3eyqcdcbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uexupzxp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hdraquqy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3myzthoqn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imqqueov.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ejngrcbt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdadcpmg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qrndbvfd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fpiawmij.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ryycgwxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sglabysw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mtbpuocp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhxizfl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3pyryzfbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmlwxlu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ahiijyjo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqcrun.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3agfofbek.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqbhwoy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mgzdzoww.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uhurxwgb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sfyimyuv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wxacwqcz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nqkuhwpz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jfjzppxx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pmndxmkd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pltcvulw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yrgpuxob.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3krgtdtya.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hidfbjgf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ogdmjdua.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypishhrb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fagkyfbw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvmhpmc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kisykebb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ncuzdzjv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lpusawwg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bmhffwqh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qqtqdjrk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3evfapxpr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ozjqyybr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wnqkqlav.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3diqohdpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3onksapfa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3alpqtylm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rcvdlqar.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3heyiqqdd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ebzfrygd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lzjmsweb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cbjvxkfq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wmyqqgxz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ekxspfig.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uwpkptzf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ompjuojb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hqpmeykn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kbqgozac.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3fihwlxng.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fklyiygk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wkctyfrh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmovqahk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bjhevaza.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kqzalijp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxprdwqv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dlbpawbz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdeqaade.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jttqaayh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cdobyvpo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ouqvdggi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qtfjgwnm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hsfihpmh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hmyexwdx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tgteivcc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3havlteyi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3txthtgmk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrmlzvxy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drfqkejb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zzglakva.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivojfque.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qybdxtwg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zlbczubh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dflggonr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sjssller.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hfjfhuem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itrnvmsz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mbchskdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tedbbkue.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpubwbyg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xrubmvds.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yacpmfqa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fmklyitp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmqrfae.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ugsohisp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mtvcrpqg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyykuzwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3piayuttf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cnwgwhth.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zknqyrjo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibdpnels.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lulesory.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfngymgf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3swdbbpxu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzssepxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3udmrnzxz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3izoqzxrv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bezxcdpo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tvizynke.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lbsvkmfq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oulvudoy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ymjoiryh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nopkoxer.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sgnvpphs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bypmmjkz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pzdljdno.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3urwasxdt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhclddfb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3inemzdms.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3izrnbpvk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3svwhnigm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mwiddhen.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjygqblv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxtyfecx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3utsurwxa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qqpyvvgp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3leqmgtel.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pywaluyb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alowypia.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3liwczyvm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hhmrerwi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xaheunmv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zubagmeg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhanxdxg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3htjjratx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbcqpowu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svimfotb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3erznfcjc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrypnnxk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lhkhtxun.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcokvipi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpcxhppd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpzlbgzd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ehjtnyxu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uljezltl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cgizkwte.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3symqiwhm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kqqxctmk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzsojiwk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tmplcchg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ranbjlto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hpfgtudd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3olymdwli.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqvurdl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3npxyxfck.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gkdbtmzh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pepcmilc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rblopdus.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iowkpvlc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gmtnngpm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tetkvxfx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nlwdsggi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfbndul.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3skesolsp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qjbjwwux.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3agexmssj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mbhbqhat.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dpllsddo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3doyrbjsl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3griieqxd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sadtdaga.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjrirwne.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xqozybwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wovnfmpn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzwcurmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vdljkehb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxzfonvj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqekpady.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okmymkgu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bhrclihv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfquxffj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3znlxlsoq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3imncjcol.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asvbbitc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlumukfb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3owqjizit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfmvqmn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dpzlhetz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3yosnrvnd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rgnqqbao.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3onsusgdn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fabrbxcc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nwpayyot.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3erwuxujv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vqgmbtvz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qmhdsprw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zclabkxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixyoameb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dbhapddm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3updzmldb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vmyoqcfb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3snlhvbxx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpwpklro.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zweaihku.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mxxomsgq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uuoxqssw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yqnognqi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iwshxshg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vknujwop.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zvfjgkdk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kbdscshk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dhhzoetb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzybyfu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uktrcaiv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clzjisub.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fimkxraw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mlukjjrt.html


<!-- 参考信息 -->