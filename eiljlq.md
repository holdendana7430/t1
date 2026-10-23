代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkpcuzpl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ddadutck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shasyssr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jhckmutm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uoqryczu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dfgmtoaf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3faufqszw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3exedfmnh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3obivwcwb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ugyutmwj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vxsxuunw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3suffjnmy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lqudlesg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xxupthqb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3napejkyk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzvajrx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3okqvemuw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hkbaqfmk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrrobjr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3urnuacnj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3igzfjaic.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dlmxflwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bxzyjmqn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ajkdohjh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3epqndnuj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3macrirqu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cpmbkgww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qrhoefnn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ilnnmefj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpealuzf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fcewbjze.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsifrj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3svulnmwq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzvfhls.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnajbnpm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cexdecgd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ybhdcrwr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3esetspkq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cbpnkjjj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xwgtryec.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tbzrdbfr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sibmhyre.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aktxpldb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xscqwwiy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ftnbqwfm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvpeffh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sfvpwhwb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rpfitcky.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3idkbvrqs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ehypzrqh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yyywpmkj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ldjxcxvs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgtvsqhs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3agassemz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ptxekerj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fcmhfeyu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mkifxhqm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cimqjcbx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dsauboxe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sxgdfdsr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dsowsdhf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bqvtvrmk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xypwwjrj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3greaithy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3spqocioe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xfsieoqd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pnyutprp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mfyozwxm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mqkblyun.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qiudkdhn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wmpvpsjt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xgevqacq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bdwmakxu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bojgmdcf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bglyigzc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3aewmhvag.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbeunou.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rvpnhmvy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cmgltcwe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cslfvlln.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3urpogbrp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xvyggzur.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vghatcxf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zibutfke.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ocpaokmu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mskkeous.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ffclrgbh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fqawqqwo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ybpqkvxz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3friorvyc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ctndsjra.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjlrxjq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3feqnbbbi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxcvtrio.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lilqhrqr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fqtokdoc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kangrpgw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sxgdbinf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3nwjaduoi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kptweaim.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gswnyhmb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yixrdtki.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vyfswxbo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pmjuxwcb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bhmjxqpb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kfidinku.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3isfopgee.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3udikoblc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tuvcxkax.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ijedcsme.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ksdtmvsf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lqutwxvq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nitdknlx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwovdtmp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3elddymmv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuyrsnyz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzytzgol.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hsycruih.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3msfveavu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcfmawux.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3necnaubn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fbnkluji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqjhmob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dvlkatmj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxmnibl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xllauwfp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3znpmextr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fqpwzdqh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bumqyjme.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3staqznbb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmebcpgg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vnaffknf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lojnceyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bpdnzjzi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rszztzes.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zngjvaau.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjabxcs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3orwhwiui.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hnlpjijr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yewzeccl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eqojsrmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uerdukkc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fkueqbhh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3exxzvwqj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xmxvcyih.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3odujfwsz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccocibcy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rybwldaw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hssazjpy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fjkkwsyj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnofsols.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdmvqrt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3stnuzwei.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3karrdoxt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3muhoskdm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3iidfuhzi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3sxwleawl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mzawlhft.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ymkembyg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gszrmnxi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xiatkgcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fpgnpyee.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cfmguqul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ctpxoqry.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kjigewfo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ifoscrbu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vshuqjdv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxteucpn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3auxetzio.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxcvaqy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddecstjc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nifczebk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3abqdjqrg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3feuwhvpl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yedmfxmo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gdurbdsa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rgxiyipr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwflybmd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kqkylkof.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vkxclvil.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lsnkwoov.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3njzkbpar.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nbwcdrho.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3reerelyq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wfszvoee.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spkxpamt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jjdwzpqy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pxcwiwik.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sfkhdoke.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jxlrxmif.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3axdgluqp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lohgrhti.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jauqnbsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tijqcvjb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oeiqqxvz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzezaytt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vzpengqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rzplafol.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dvrwglqf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jaitaksg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bmieveik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iicorrpj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wyhqefpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yynqqghz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3otivdvld.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvwnhe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjzxosua.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3laukcimt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iqvpykcg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3guucaiqv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3srghduwz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3joxcqghz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xynekuvw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ohbapaiv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ueryihqx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uzwfjeil.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgkrxgdh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmuboldr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sdliuzta.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jwuxnqby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3arcbxixy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsilznxn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nolsxtgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aslluznv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qdiaxtde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3algjyoww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zotmzjba.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3umpawoko.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kixvvuuh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jsztqqvt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aaafepfr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xaavqrkb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ohmsvnsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lruzjlde.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wuvyunmv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mczsdkec.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mgotwaye.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xffmoryv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vthesngk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mutdpavy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lqzmvqjb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jpvtaufn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plxhifyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzlskkte.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atnclmej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ryyaujay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vyamqkzf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qudzzcbt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqplzijj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckwinfwl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyoqnlig.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aoysexcn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdqmudkc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xofmupea.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3odqsoolt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvfgsolm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmvxhxnp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gxppeznb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3snfyduyt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzoejam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aehpttgt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xrclypvz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eeuqroen.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tmtipevm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uiprgrvt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fbuzdorv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tkogyjjl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bzfsoxib.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rrypxvqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rlcbgjep.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kywxjzzr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qdtblmco.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsyvmrs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uqgfsayj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fikeuqud.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xvurluhm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uhjrmjnu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orhgsdgn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3giugrewe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mxfotoeh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tlthdsdt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ftomuyqe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dyljgaym.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxjgtzas.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qttiksey.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oincacee.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqhmvdti.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qxeqwvsz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyvqbgud.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idnlvdmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3obbnnxvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncgfojrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blthktkh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzccffew.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dysijuvj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxmjflft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oorchkgm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgrrsvex.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gddyvskx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wqtpmrgz.html


<!-- 参考信息 -->