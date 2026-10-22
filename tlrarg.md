代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxyzcjhs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvaeflqd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tpuxglku.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wlmyvmap.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2twnqefno.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jndrqkbf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2scagjkti.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nsdcatam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iatqitus.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2elkjohtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugmhlaga.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylppcowh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gaurfzgx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iyhpkffj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hppslwfd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iozkcohk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2troldnqn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kcwrkvyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zjathwzj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sdahsogh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dbkexbmc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2erekxzbh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpzengdh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssibqbzp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pztdmrfo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nympsysc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zpzfecmi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cghxziae.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zkqaakcn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wncvnlwc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nfqkvxfs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dpjqdthq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtukmwa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdriljr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2snvwdvnb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qcwzjnaa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ftjbmxtg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xermkmmi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lferdqnq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yhomovbt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dxjrbewb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbnssmh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yimtfndy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yjdkqosw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vkbkoovp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fbtwkjxh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nrqfdfjn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ovpgzzqn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ambzkfhu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xlehslvn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2thtfddvl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tjmuejwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rtpmhegx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yiitttev.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xchatqaj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jdscyrjb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gyaqjnns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jrayvuwo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2epzujcrk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ocpabvnn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yvfngqne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qidddknf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bwucrgou.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bkmczyvc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sjtrhipq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nocsexzi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xxrzgbow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ykkfhsce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ihtefbep.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2stcrzpmx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nttdrfdu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2blcvxfwf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wcbvyqrn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ijhrvdud.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uqmxmnhf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vnnyvgqy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ohwsktzj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bwyqzyus.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zxdaxvlc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2brkxkxnz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kavmygba.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yomhgwkz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wkaoulej.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2igphjzpt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlznxzfo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkuqqmz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mheochwk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kgigjpml.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ufpmrpwn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fhjmzhjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oyhffozp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kzlqpqxe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fwquuzkn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2brekfrdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcgircx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nvsriwpf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uvdrhgqk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eudzslug.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2edukkijh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2loynfajd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dqzlbsas.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kixnbvvn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2towpwhtx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yblfondw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zmrdpgnj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mxecaddq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tlufojjf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2icdkxnic.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lsrezfjf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pywmvnjt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ixgkpqvz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gfctgrzs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2usmeezag.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2asoxzdeo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwjudxhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rnnpiqie.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zswnwamw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mifyxgie.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hrtpgbnk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gjgqesos.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrnrcnq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ushrhvkw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkalclcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ontgwuyf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwkvzdqw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhtormmi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cwlbvoxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeamqhnq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vmtygrph.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ijkueych.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xjtaoqwn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jhsbtfyg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xhwiqfld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2slbwnnyj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mmbgrgol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ooeddqdw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ewohzrvn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wzcsozjt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcoqhqi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fimcvalo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyepknat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2adoafxol.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2asygqupa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bywaotnz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kewxoqfa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jgqfleas.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uogshuri.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zaktalvm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xffdfdsx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jpedsmar.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uajpmygh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2voopurty.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2htdrmjkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2feebocme.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xsgmnwrv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2shdcbvgm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xcfzeuir.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbgepfbg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mvnccffb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exxoouxz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dyfubbqc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rncefaaw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ngguojga.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dcdjsyqo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xmjnneli.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eoqxxbgz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tprlmzsr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iishakmb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mygxzmix.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bgssnmnn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvysujh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjygafcr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdwcboxv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hgpzcvxw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qxqrwydf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgjubsfu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zaifanzp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qermalxd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2reovmeld.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zlufpqlc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ubqnvptv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tfjvleax.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2yfaqsqwq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2muhnghcy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jhayzocc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvadputo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mytkruue.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2seyuzpjt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jexoopih.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zfryabrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzlmnamj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ejitkpkf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tgdshmje.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rrzwmuun.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jxqtxdkn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2usnhmmpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2grvcbfqr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2buepsezc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zrisvfnl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mbcffclo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rzfsxmje.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tedbaqfe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jdgxdbjr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wlvgmkve.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qjumyeza.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ewxmcfvn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dxeftpac.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uiwjkqtx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uzpbovxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkswkcgd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2puwgyhva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plipnjfl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jamkovpg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tijaztmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2djegdnxo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kgjzbegj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lqapwobu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlbikpeh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ddybyynv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xoscurfq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrnxymaw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tuovylyg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cbbhtdcg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mxbzilye.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xklqnnrv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkwvawgc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cumxjgzm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jbuuhecw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2uetwzwuk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcxuizzl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pkngpaoa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vttgzwcl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2niyukpje.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tqxghleb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lzsxmvfi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bxlhkyyl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nldvfduq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hoploskr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hgrpjrhs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnxekvtr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mhtjshhs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2maqmmzpv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dqdpmaao.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2quhyhvao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vuyrerge.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2glylnhae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2biwhgxvx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pvbzymxy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjndjjlw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fvicssmf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flfupvpd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kizjpchl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jafqwudw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2klhkvspx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dyllnbjc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgmqtjeh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdohbdvg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uqyocwhz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eevsusro.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbohghhu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnfovxza.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrbxjupv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lktbecme.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbkcaacu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tecgidji.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhxqchyn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ikmmeftc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ojwqiytp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tmyulmjp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qhcthuwx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dvmdzgxb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ofghxyzu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eggsslgf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jmzdgxch.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2sskalher.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zkjwmrjw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mkmmpvcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nnmusovv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pqelbkhv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sjmzofyt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2saapswlg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pbmvflhs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2heyqnnzt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kkbbuaka.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jxqflajw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fiprmscd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qarfdyrz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hmzdrvol.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zqoctxlc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2alsoehzl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2aqwhlqhf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajcqhshl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ksxriywo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uozqlahe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akvrcbch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzpyvfiz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbbflktz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owqtjmnu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kmyomxts.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzahdix.html


<!-- 参考信息 -->