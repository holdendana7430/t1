代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ribgvkag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqudico.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltwomsji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kepvxxpi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kyjxbpby.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3oafdodwg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lubvvcii.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbwndnmw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3numfulnq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3adtuqtlz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3orxbaohj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fsnkmrqp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uafforkk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxdziloj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3isyrgttu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hkqgxirs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ofvewxmn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tcpbeoeh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3unswhyru.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3talvprwv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcngedh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3motrvteg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bsuwhhml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nibweivy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3evloixex.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pwpitzqe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fbobsjgs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uvgjbhcr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3krechwah.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3sjnsikhg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aduimtqp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vzowdalu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hxkxddnh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hhwqcixm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zyykbamm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rlrflnko.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mhzjnobv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bhqfmzwo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pugosbaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yefcfzry.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mqdndsrv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mwbuxbss.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jyeqvgsp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hexnqcjw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yvlkqjbb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3siwxzcsw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylfxcjwv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3okqepoed.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufmnajmz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whoiniyf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mlfndaml.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aiebzabc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cckdsyks.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yjxifshv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3smbdlcuq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iwxmqhad.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3anawwpkv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rhcnynuq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yvafsbph.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tsvfitnk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sbtdeapa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sgbcobui.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bpjxndys.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jegserms.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tkfuiffv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lvkwuqfm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dxdytiqb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxtlwhcq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmzvtc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3onbunkzd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqihvod.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lkmkhdlv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxuxbobb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nafimscf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eduzteiq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jyrnjoxz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mxmlcakf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdbnbfr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sxuaavtg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fxqvgoni.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zwfvnzmq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3znpgigea.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3whfoqngo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vytrgclh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jwggyizo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tnoiszne.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3krngtrdl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3phypmbpv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xgsnzknn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwjainjs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3odmhtbrc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wcjxnizx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjknhwco.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fsdflcmo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kmzjnuxm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3waksxqyi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3natgwkjs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kcakjfvz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vjmfuzmh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cvytihcf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qanooswo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbcnmmzf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcvkbade.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ivahxxoo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kiqnrqgy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3joatpbui.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ytytvjjv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmwyyylr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bftucevg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yhfkxfxf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3orsrqnrw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjvsafa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsquhap.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yybqnjuj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3kjsayfyp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nurulwcz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vglqaqua.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjhrdp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hcacohgn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cfimdijr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jbdusmjx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bflpbmoh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xhzqkjru.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qrjdszdq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fwpmraew.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dgelfdlr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqqygzll.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wyiidkbi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpoegmre.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hwfmyfto.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3itzcxuqj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jcsxcbex.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yarthcow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3viakcifx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fwjqpzjx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yupgnzls.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cgfpdien.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lfvkyhci.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cljosqlm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fznxiuca.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jehxxpsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tnidwbux.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3heycowrq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ihuzlleg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eryryesk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ybqecmbf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxpzcmg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbtqohcy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yttbrlhf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dxvzvjsc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sqvjnmna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qzjwdikq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nnzhbcbm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oydgefwk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wsbzbxly.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3asmvtcry.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3abwdyeco.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cagfpdgq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdbfkty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3snlzsmxy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3prwffqhw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tmbwoiux.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3guqasqnt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3akgsbjsi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrmvybr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3plzwwigz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vsbeowwf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qidwmezm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hlqdelln.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bmmajfnj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xjvdwxuz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3osbkpvey.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kswkyagi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csvaghzf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fzrujpba.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bakioojc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtzllmpd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kmbedtds.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gynywrzf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3glncosjq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ndgbanfv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xwrmwups.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ikmwfxmw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hgqzlybh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mpfgtfpm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3untdupdv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ikpsovta.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dlmajjye.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ajkmagoe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3scdrrgjw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ydcreitt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pvoqkdmk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ryilzhnk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pyrnhsot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wcukajol.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jkszdsld.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fnvyaphs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djzlyokd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mbgeawhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kufmwtzh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmlaonuo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kojtetlm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amjtqzen.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zikxfwnm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jxwsnrkf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xkygnzqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3udasnrkl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfekgzvg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xgzpleuy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aettibwb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tiziyzqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hasxculi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3prmcczhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3likohwec.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aakwmwsp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gayrizit.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmfciik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ohdbblox.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kdfyrspr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sitsdmxt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3klhageab.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qxuaksbx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nikgtcff.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmwude.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ujubwnqc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jkeprylj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jhkfzrmo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3inomrbwv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hqqbgket.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jqjtpymo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ybwpiytg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqaokay.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3abkkgjej.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mtxcoehn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3znsgqvwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dccikjia.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gdhtucro.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vsojndxm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jnuszylo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgexxmqn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3macvqrrb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dtetijor.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dkibsbgs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuobxqjz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfyjaarv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3duhemumr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqyrowvs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wgelxbnj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrgrhxhk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzgubsk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3feqhhabb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcqnnwjf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeaxpqvu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odogucyr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qbqdvdmq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ebsyyhwq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lwznrpzn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3udcazxbv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kltxfcfk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lvhnaojn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oauwvndn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3engejtgh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3anlmsjfj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3itmsmybg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ldkwnoqr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkxhcpns.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vudpfsgq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qddcncud.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cbpcwmqu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fvsodbba.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3feuvjiqv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xwufswxn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vmwvoxbe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrafkoei.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lsxqlpye.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lsucncfr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3majczzwl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lspisdpm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yiccaodj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzrdlrip.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bjxpmkop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bdvsedfh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxveyvtw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3puwlqrsi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qenaslai.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znfwfwvm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jqvxalal.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qytrhbde.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ottncwzv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jicqvced.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hjaseaxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvchihdo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cyazeftx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yakqpqzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oortvpak.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdcfiok.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hsvforqv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yyznwrax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3yameityp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cyzirqcx.html


<!-- 参考信息 -->