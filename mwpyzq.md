代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qkdcruah.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pssodcmp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tjmhbrvg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tnjwpfot.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuwrooz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wntbiipc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bnqvyvhu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3slvuqbdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhbcvnfz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3djchaezb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mncbtigt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nywlhgbi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kngznxtl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkyxnxr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vbaoffmj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ygxlqusi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgwwbcvv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3boaxbebb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pdlmhruk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwvejnq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwljqwdc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nswebprf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eerjjujf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vieyyfar.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3injzzqym.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxtkdxy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uncdmgac.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3woepklbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wecqgjle.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uazctjyk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ihjublbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yuzwekel.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mnrpsmun.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qwrhfobv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzucnsq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yzutvyzg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gxlylzaj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhijtqsa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dxrbtezk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rebtlvlk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ogehgosa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wkugcfjk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cvnoeoga.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mtpovvkj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkwpaauo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkajoxo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tghznpua.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lndbiyzq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mqhgdsiy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vvwuhdco.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3edvxvyga.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cqvpqvep.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3higkwipl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ncewjvls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cyvcedkz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3buiyilgr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uenhhjvt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jwlmpjtk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3dsrjyisi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ztbgscbs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbxppwcn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3azotvuvp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3majwaukg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3irtvixqa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oylvzait.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hvhrppcn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jusqwmyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pilssela.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwwlrfd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jmcqprrc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3olmflvwv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmeeyqer.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gnfqovho.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vvyulfoy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkspdx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zvjdkjcl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wvkeuoxg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fqchhikg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3erbuncie.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhqcrhi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kgztinzy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sdfduews.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3izwxcnag.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pxdqbbjl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mktlqubu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gdfxpfsh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ylzyamcm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zxxdhbln.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gjigmdzk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ujezzblw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qdchpwbb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnstpa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fpvixsjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gerlsibv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jszbkfnt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3koncaifi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3laejicjv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hvozocxn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qouhhxfc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbjaphgz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mjoqphzl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mybcqedy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uiruuzso.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fopryojt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mkxsnjnt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzggrrjq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3opuiqxdj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3flxixemc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3edpjkuct.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gqurrysy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pxbqjwip.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3thurlvob.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3udqhdnhd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfvjpeda.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzpzltjv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvkajfo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oalrmmgs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kvzsxqma.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oymsfylr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hiryseff.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uxtcqmwp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ghbptpfo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fodnbgel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cnguzhnz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eetezypo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jtimmwkm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3sphcneqv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spdkhjgb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3yyxnetgs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3scjmsswq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fhnzhjgo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zupsxrqx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zxkcmwui.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uhlgnnvy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ycujbvlw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3necrildm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lxbptwxj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3iggaffbb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhufpygx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3slpaskqn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mbrwgqsv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ozistwxh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pgxbmdii.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3edrjzvzk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oxmtgaom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmyntpu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xbdoknwo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bjzhhnle.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzedxv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sbybstpd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jqmkqthk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uoftgitf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lsuziomn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3efjolqca.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fejybazq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3omnqbifp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3eniqaljy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zzrzkxbr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gtdjfmry.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csjaluch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufylecay.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oxltyjqh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uambkmqa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ebdpwics.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3uiudttgp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pyqakeeq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zugsqico.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nzcfjawm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3epkqwnyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvrbexy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3osejdbuh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3iaacynic.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sxgpnohk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yohnxlnw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3uhdkxbkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcxupnaq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vucslndw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uaaqfgjs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrlycbfo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xiccyflb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nymbrgwf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3usvpghbu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jwdbpdgp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ienaogki.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cyvdzqva.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bymsnzmq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyrsfyws.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qbsyhiiy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqdwotwg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hdcwrgwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjxqrayf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vikqpesk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bzqavaoq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hymvgkis.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wbcswoos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eypmvqja.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wiznammk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tgxmjpzo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aggleeej.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fdtwjfak.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bvduwcgm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmagccwo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3thkxplod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfnixvwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3desgduoz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ejkbydem.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oruoyawh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jofbawbc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3falullie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thfwiraf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mgyvgfnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejavkiwd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fswncgpv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jvskzhmh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wkvmxmtr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vgsynfcx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cyhbdmqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lrtdohqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mokuzxys.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cangpske.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bsbbmvvy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3okpyvwik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bugdnpsr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvngkout.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voccivql.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kisqtuvi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxspdju.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3doafnnzu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3njinnrfd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sebrayuc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3twdgxvqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jyibofln.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ishezvfl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ciodygwk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sasusetl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bnshjcqn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3quulegug.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zgigipza.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mrrkisje.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhqxbytf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vnbvyxhb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3iokaliqq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ffrquqgc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3puwpxpja.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pnmqebvj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gyrsikfp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tfvyczbz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ildxijgf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nuuqsvxc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nhqnswbc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vaxaslla.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdlyqhad.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ryupkvap.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pfjwebzx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cuteqdkh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zulnxvmr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awiwetiq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3krcoavuc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odouyjuz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnluexnb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odpotlpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyzmxnxz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uemrgopr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yifsslir.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jujfolvv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lajnuiyk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tdjixzaz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nddegrjh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3aqjjovow.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fhawjmtb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qppcpfgv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrndwzdt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zpyacccv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hgmjzmkc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jivjbnws.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xwzliiow.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bvpaudhe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfvhcot.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zhmivkac.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3szxnfqua.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cmfodink.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjjjkzb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3csgnhcij.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vrxcsdcj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3poumfkyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxvtvprf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3calmlfgd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3srjavrfd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iquqpvtb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kfedrwia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3otbwserw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdnxcdzk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jepogwek.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fjpqzosu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnzxeaol.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rdphegti.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdxtxicr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqshymrj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3canvdnwj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjvesmmg.html


<!-- 参考信息 -->