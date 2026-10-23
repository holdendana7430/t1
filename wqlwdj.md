代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mkfheugx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sospkhbt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zasyhbsb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dmuznofd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3roipofax.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3upfljets.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hwbvojzo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrzxqlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbpilhdg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oqgzmwcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trryyfts.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3agjeufxs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qpnpzapk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqlvbbxi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eianlazv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jdohatpc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3boppfpdv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3afcqogkt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rcykjejo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3obbpyywr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgsscson.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3thvivqjr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iktnvnyh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mewikdgk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zhtcccte.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tkruimji.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnzpnrut.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3egffzqok.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrtaaz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oyflvowr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sluyqzrk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3izarlwpy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbuemqsc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3glhrupfy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rlwdjxcy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ddvsllrr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3dnykklng.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rvuhhmkd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3homptfbm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bvktzjfi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yvupcvye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfqxjvn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lcuzfgkr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwgflqgu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ubatvgeu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ddzbihox.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uchltsuo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qljqhhox.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wbwukskv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qsylrwmb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mtxznpua.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3veoymdoy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aazlyyub.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zpulmfrv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwtzqdu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3scadxwvy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rrdyqfsa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbzhdec.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xlmbhqev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qabntxrn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ohaijpws.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fnzkhpdv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqemgzvt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjhxdsa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gnsutspi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kqsmobji.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3apuhlkae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ieaxljoq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xpcziaop.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lpqfrkfb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tuqfugvb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ieveyurn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cmvqtpgg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tccegedg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jfllwdom.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xtgjjepr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bffojyhx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ivczxzks.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qgwlvnza.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ozbppkov.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iidojedv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwofywmp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dbzfqlyt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xocmqgop.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmtvyfc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ngevitky.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rswljwvj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gdjzbplt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ycfuanhp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oceazvgs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3efuhbtxk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gtjrzhkn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mqdaqxbd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgkpjrso.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ixodaadf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbmjjcu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qujwarie.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwcmnui.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3usgixtdd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qkwptltz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zzgzdkdy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lcfzqfby.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aafzpeal.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nmyyevdt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uumldqiy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3npdpaeje.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbdhwau.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zhpdebik.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3edyollwo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3thgnhwuh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rpzwgnuu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dhaqhnzg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3esrlnghj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctwvyqga.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zpxpxxqn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mmzshdsg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vachvwai.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ybjrhnwm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rusdofll.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fltchfff.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3aamdzjfc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kqzgpvhz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3snuyzwqa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xrswywcz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3giyxzgzh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yutjuzyg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sgnzveue.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iholrgzy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vzrkkidd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3utqhvejc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xzljmexq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3axesfios.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jscthuqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3drfotmjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gxpbhowi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bskwquxb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qphkdgqa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3erzeofnd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtugadjm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vkgpixbv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dpehsrsv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zlllummu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bhuehoaz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzhvzgd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydgjnobd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ignnynmq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gdtblzsu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ozhbvvwo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jtqauuwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qkujvcvn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mwlwenrr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qrexjehw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3balmqdap.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ariincjq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wvpqwobv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xsqccmkk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mtxnxcey.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qsgjbqlw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcoukwwm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqkvsvy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pxgodkkn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ljtoabig.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hlloqlbo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xpocrcsa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ijhibddf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rkxpogub.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wfkfhdrg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wljuwgpa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3slxhpwfx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wkfvfpmo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ylcbvdoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tlwwhtwq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xghsrcth.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oqjskbde.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tetrhiqf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypqiklfs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwohqsc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kyhgryrp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3befwvzjj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tktkheoe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jvijybmq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3drbbszsu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3pkljiomx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3najfgtkp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3snxadqgd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyjhkwne.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nmalhqwj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3oewamgsu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mwsyozcr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lodysdcz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lphhaxvw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fffxexvn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fdiznhuw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3odvqjqaf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cigvhxoq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bcaudttt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdeisugk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jpubhlpv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uxxcbfxd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fmmdulwl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ppunitxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ailzjzbt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vfugrbck.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gzypavla.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fqrovmdn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gplfpfsg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ytsynhce.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3duufpqov.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3valhkeew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsvqpzcg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3prljjtwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcacmaqg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xipfelae.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gnofsbnl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gcscrxvo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mfhopkbx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fjxgnlhp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mygycqbm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fltuejpq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbuzzqgi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cfbgsqny.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjuait.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gfvlkldq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3asvmzlbl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcvkjhos.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ewsettmn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rvptjzdf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ehwvopef.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mpcfbolm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvfernae.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bbfposba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hzrbqnlz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smolmvhy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3prljifko.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qhoejrdk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nhcvmzoi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zdxzzssr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cltfblnn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zqrwaexn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qznfdxlk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mthnlcqu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nvogxzlc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3crywhrwp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3adenyqdb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vnrgcatx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vddzzgxw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3schrcosn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3emasqpwd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bbotokhm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nehnuagk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3knpgkmvl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqyajhob.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkmaqink.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xmkkolwy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qxmaseeu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnjimowo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hpergtev.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bitntptf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pscszihr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnhelcbi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwgihytw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szaueami.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xchybnlf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnyleb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqavipin.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwtsirwn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rlergnyy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3omprkqsq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kuqlxzfx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vyiqkjgq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uigopdzd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qysvzzgd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cploiadr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3oizhjjfv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3roerkflm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dvqxukqy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3brtinkyb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jvznslod.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qmkyhtdo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ypayydtd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eadnygwg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fiwdeyep.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hqelolqf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gnekommp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3egcwffbw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgficqlh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovidawwa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tlyxpptc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xqjgqmuh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rzrzaone.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yyyxfyje.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjvnfqeg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hlvcrfee.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3stalqssc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzwhbvir.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lurdcvnq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yznsuccu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svaqjsgr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tdcpbebq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgwoifyl.html


<!-- 参考信息 -->