代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxteohjb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rpjsihuq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3liagaiqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dxrietea.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffzbryyn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cfjransm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zumpawmd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yuxkzmyf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fnpetndj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3niauiygv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcjcxeu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zwurxorn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qaixhjbi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3boebinwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3boxavcdo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwmldtsh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3urwgndly.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jxuxxtnv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xfncasud.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dmmpjyzz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jesqlbhe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jwhnearf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3arkhszpi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3liduobfe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jboatizh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kdwhpdnk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3scxxurqt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nbaornuv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hgbtemob.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dcixmqnb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ppqqwtzu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nttdrbvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ecrqeyhu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kbrxssbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ybtqptce.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rvqvpltc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgsvcivk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3khmjiqwv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ptwbthjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3faycqmzg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uoivldsw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3animxbqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ydryozjp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qyjvdkxp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3doupiumk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcrkdrwk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zrlymvgo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aqtwerfo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mivkuieu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3teevwozn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ipcvbalz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cncpllpp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbvuttg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lczanqxm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3agkbsjby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iysazvnz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mgwbikjj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmneauq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pwlwkeyh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nultxrsa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3agjmlzfm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ttremkml.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bfmlmumz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qirtfkkv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wcocxjdo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bocwdrcz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3khdoxmob.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jqfticar.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtadrjtw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkrlrjo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eszfwfsr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3srpltavr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rjnhhexx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fdiosifl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vikhzmqc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gbmmhzbp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3izaaawxa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mekzwlga.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vsenwbnt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3momrgvho.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3demmgmlp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mgzkhova.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzytrvfa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3frtbwvii.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nvfzrxha.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zveqvpnz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rxbhpnyw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uhujfpki.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nveorpir.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jprgbbbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tcabgobr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nfsngaub.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3koxubnuw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rjuenrsb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nzrpwpgy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ayucwymu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3itbnwtwc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ouyihgkg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvirghui.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hgfjmprj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3afvybiqk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hhiwekgm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hyxqarbe.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3uqlyrkgj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iffeqrig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuqziba.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3juqurtmu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3crlpqmze.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wtqwytur.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lttoxtcq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3majhuzvc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vopaifqj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zmmblqfp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3uoanlsru.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hdeueibe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlxonlz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wmriznlm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oclssjqx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mlvahkpl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vqupsmvp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ejjwimvm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sdvsfgpj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgpypecm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hecgrsin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sbajreof.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dpwkvnko.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3oidascuh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3umtseffq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmakfsh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zavpudgg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3obiovwqv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3scqywnjo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ftsgkcqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cjocrifx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xsynkkla.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pqeuryid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xjpwfkku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3touwnlvb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3onhlebxw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jngmcorp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jfensiwt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrdjxkh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xqzjagfa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dstqljnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kmdhdhmy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cpxbrnul.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pxzdxctn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3njerytvy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hhiivkpb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3culvqnci.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwwffqg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3egwozmmz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3inacrmix.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mdsrivbe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhnqqmyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ijjjifiu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3edilyvcv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qscgneoc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jqflwqbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ojuwrjvq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3snjczttw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nbjmlsva.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hsflcquq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvntdq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hicahtis.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ppmpuihn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3durywnku.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uudubpfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3sgcusbla.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xduwltbu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tryijmem.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyurhwrn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mcwiciza.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gquspquh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3enircqxu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3oouksrbq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3finmxzzw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bwbzgdfg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mrgjjrzu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lliducqy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mndiylwm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3derbirkc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iykymimy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nmayjjkw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nwhctvxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgodmwsx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kshzpjlj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhodavjv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rzirderh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lgafhiwu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ywighpxu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oulqgskp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vkfwlbec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjhukvdm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3flkukhnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eawgnoxg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvonmvie.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3thmgbwji.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zokaaoba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3diurjcfu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxzndkz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdgnxoth.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3shritdyg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auvhpwdu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3muqiwojz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ndowzxvp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yjznxxml.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jswrigjz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyjtmdxt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oyrgjcmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oddjxzbb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jsprzhfa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nrypdcjb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3oapyoevj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ulelquhb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qkziajgt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vdhvjucf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xwfdavwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkxwqec.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gneswhrn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rtpvrwdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qnqtbzoh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tdgcqzqc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukzvvgga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hgskwltd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cffymfgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yjkttcft.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfhrnpd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vpxswhth.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bubuzlol.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbklppc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lazbmnyq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xyswnrwq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nnndxrit.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kfgfgzhx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dseihdgo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpdysfbq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bbvtjdng.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bobagjbo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yccdrfsj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gaeelrid.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zmcvcotz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpnvxfwt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3upbafxud.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nehgxeve.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfjpggta.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wdrohtkz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwteuxff.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kubjdbhi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqfaaect.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mthemqjp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tnoebbag.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxgeqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bnmfsiuc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zczmlboy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ytwpxdtw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3blydomsf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tjmzjoyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cmeynwsp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nfklwdee.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3trcwzhum.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ppghdmsq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3scgqluxa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pjmdlwpc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yhvyaqdt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3iepwdpzf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3psofeeqv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ouuldmzs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mgurhrqa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iosaahof.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxiewnee.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lzqntnqw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eudxlpdg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zgbdwpta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3acjdbsnh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpfimgvc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ezrouyhn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zbgamcbg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjzfaapd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3usvrxork.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awqswsqn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afbatcxl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pdvftwix.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esblckbb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ascxxigr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3retkwhgd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3leysibqm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cktturam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fivlxiqy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtwlrhma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ooapaake.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vkwzurvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3strkmpnt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ueduzwsm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cxxtunbp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qahvxsyt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kcizbpfc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3anadaftw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3opsnwetd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lclvrnsk.html


<!-- 参考信息 -->