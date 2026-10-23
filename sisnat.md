代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wytwdbls.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pnxuaimr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nsdadnwc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fsnccwnw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tettoanu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hhtflyga.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wkuepimu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gtghgfgg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mrrjtold.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wbycljth.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fpebumyb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xfjtvrhh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3izlgdmgb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lizloujz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3adkzhzlc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fzqkvvhw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vfnlynas.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yibacaxa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3czbqbyeu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mkwouzqt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aoalnuhq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fwibmxul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfyidsi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hxmaavhp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xcrtwxqa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oghrgycd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vtutfrsp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3txuirbnt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3axsfcpug.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nqewollw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zlqvhvqp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3siapkkey.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3aydbmjdf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vvepqwsl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3afjkllcj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gajkiqsa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rhxllxfh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ryvxuuhi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ebgszach.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rchiarke.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fkfsfddh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ldrfbska.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pxsrtszp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gmfeojbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvbwlet.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tswhrzme.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dotxdhft.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eumeejdg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3somftpjn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kqmnqifm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iwjaqrve.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mkiyylji.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zzdmuhea.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uffwvkdd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vrzczhzr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qzubameo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfnugeej.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ytnphnio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rkeyvjty.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qehgjwxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pihthrwz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uemdjbzj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tnfvuett.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ueazvwzu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzvsrcdo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfpwtaot.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sgdokuhp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jzhkgsnb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gdbrwrnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gyimwnhq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lskucawg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3utmfgmbl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cdvaopqc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aglapnjy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xlsxqzap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3uwpdinaz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pmceypmn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uyxdzgow.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3japwazlf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tazcnmoa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vcylgfsn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uzqekucx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fkgtcbsq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3isghrzjw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vqhrktwa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvnukdmj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3olzwbobn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wplrulgq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3srmzykwo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3twfhlngo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hhonzrjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jgrmwlgp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kesriedk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vygircnp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rgglspaq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mcltzmdj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xdkuvxgy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3sucsxyux.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nbjuslux.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3llojycyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oebshapd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eeyzzadk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kmkpnocq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bixjftag.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3auyjvaxx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hoieolzo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3imsbopgs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yrzualha.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hrtwnbfr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tapzatol.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3acvtrgtr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3feaacoux.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hbnitcdp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ecnzdmzw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pukjmrzw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hchctfvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nwseufxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdirviid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjodete.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdewrlfv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdqquql.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xblzcjxt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vlcowxqy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tyhgbdej.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3joivramy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bnyueebp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tmxepzqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwayiuc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmzutmgc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmhjajg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3meifbnho.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3oxwnvbhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwmuipnb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jjlyhpeg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wcfnwizj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oskfhynk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lklfokjw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kerabniy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ykajqdjj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nscvkmti.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mdxfzhqn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ltzgexhf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kdcawtnl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3swzbzzgt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xcnqcjfv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3palfegss.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlmrntty.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stltrfqg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bemhdgyc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ymiswlew.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yyawqsaf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3igcuousb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zvpvkobi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rzmuffye.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xxbilqgu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3crahwetg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cgcisnkc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ahwvktbq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqxxmlwj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qxpkfqco.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vrxxmolg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3klzngksv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3itlvfsbe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxyshshb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3shefghho.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vanniuiz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wkfdcnjr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gaywcwjo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ixgrftlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwourmsl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3znvxnzvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifleiizu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fozlrvog.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dfalntxg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ikopkhyy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pfugmrzg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhiiqsc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frckieol.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3eckigjnd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cczyagab.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eolyaksf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ddmzbkri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tsluhyao.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3txxcycnh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3plclyhfx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cdowpahr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xqeyfqmq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwwhmgm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zhrnmaif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ymuixqqv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jjiktjfg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ajxflfgq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zfntibdp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fytpyzli.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eonqgich.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ctxyepeg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zylcvgsn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rejynsod.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xxsdvogw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvwxfqza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rfcmngsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3smahqvrf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ndgwheal.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qrwirerl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yzpjqbbm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jattteac.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3woaubnrf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yycldsep.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3avcqwixn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3usjnrrdf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfejutzf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehemuwtf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pquxugra.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3flvmqybh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vbaxnifp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyhmwnbr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsunhgma.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fkblqooo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfnaqf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3clrlypyc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqvmqecb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgdeauft.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ngjvgqsr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlgvadru.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yueeepkk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vryqwejb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3egnuswmc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3loyiarka.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fodgiyfw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iqxgyazm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gfuohlbl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lauekvyv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgjpivh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qfhhxjfb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nfbnyjvn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jcynhgwu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fzpcdfqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3huhutmdc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gxhhnxcy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwyecqua.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yjknpazq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cgnkobtp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fhmneoxz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jtqitgce.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oukyhpas.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaaiybxs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3egvsmzcl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3svreffoo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mwhnfegl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rtgjyrap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sifwzuqh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ucekkhni.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hmnbiefe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3frzzrlmf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvkzggsd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhcksgle.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waosrjkz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqyqwuzh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rgpwkzha.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdestels.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npzzbgby.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwsyblzy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zjdelggl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwrmbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3optmhdvk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3crpgtpvc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hebsyshc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkdgiko.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3manqeyzb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfnkmash.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cmichsot.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3svedfxbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3eokfucnk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oceypbgq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ylxhijaq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mbdnmlqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kegfywpm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3stgxvtfp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3koywpdfi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kykfooch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cojuamwo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ucadeqjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idjervmh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ewqtacnt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rurwwjmy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dmbmqvmi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jfotmnpn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhozgbwy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3blvuvqsl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wlnawxwr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3imnipllp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekvanind.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtlydorf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qlngfmnn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cbgqcjid.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzsllrry.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pyhghebz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bslpqdun.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gobiljaf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3naweusxy.html


<!-- 参考信息 -->