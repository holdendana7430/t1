代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ogniclwx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3chxynbea.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqfoydke.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xsyhxgvh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3erkbjaum.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tvrpqkzl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3norlqdlm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sbmkymwa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ckivyhjz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hnuqswdl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fxkhunfz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wownypff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfvivobh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iowysoyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wedyhvzg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wtcwvrgd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3angoqpmd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ockouzsy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krnuwwyy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3neiwmpgt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvlkiqkc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kkqqminb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xzizlzqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ybljufco.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qnmsrqxq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iznxutzs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxugeus.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lfmjvftg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qdljsyzl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3erpelkmh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dswkpszs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zrotqxul.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rbiesvle.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iemolhxt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vzfkvkgf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3icvbmozg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ppnoxbap.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rzhgmvtv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qaevmdjt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ryizceig.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dqleytos.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dpxzaism.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bjlcyrdd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dofcuetx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cbtgcdiy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gsxdqtfz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xqwkfedr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ilpdgiln.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wxedjhla.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wocerqvg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnmcsgyx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xnvigkdc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rroyrwvt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ubawwaxh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzofyhos.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wniuvape.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yokcihhx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3olhprpxa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yooexlhh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rxtsxkxe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zwpagdre.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwgzdbw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sobpodyj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdtjfotx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rhkmltym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ixxpzbdq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjtgkcx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xzxmqgji.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rpgefbxp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dfdvinig.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zqrbynpw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xrabbxcn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kjlyzcft.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dqedbqkp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hbonzbnw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzoqrdb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3eclmpyyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zsiwtpgr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3oehosywl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfwghnk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fxalhuhk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3crpcjxru.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3swuzpgjw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jvlauqdj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3trzxuauw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3psqkmuuz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rjluatfx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3httppuct.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3usfnzjbk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqyitrss.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wmznovoc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3myluzina.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sshjeogh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lsrobrxe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bvcvxoim.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pejyeqmh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3reykihtn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mlbcfzmz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqiwhie.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xhgumkbl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yqkxabmz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rybshyzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fbwwklqz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gamdxxrp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qywhlyvz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ohewqcqx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmdhif.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3brciwzwm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbxkglj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tnkbzvko.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vmaglnxg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jhsiikdo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qtlkklyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3juywdwns.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mwfayskw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yoxbmkhe.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kbzaklci.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wrbzkbos.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzwytwax.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hmfazfel.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kmqqvnby.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qylpffos.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ivnaizfj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ijmahnwg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rfdyeikk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3otvjjsju.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3roguboch.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtypybkf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwhjdpp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ywxashbu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsyrpem.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eupqqafc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hgohzqoo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jxufudbp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dabwxszn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tsxkzgim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vipmflyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmkpovn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bmfqfhis.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ggcgjgca.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tpizcnbl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qwhriuea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jyxswkoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqjttomj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhhfgrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bvnytzma.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ezqdnvqf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kftudyxi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3siulrasj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snopdjlt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dwlcelmq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kstnfnjg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sttwofpi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lgehjhka.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yveowcpl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxcwzms.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fsrwgggx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rwabfgqf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rsbzhojh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rindnxqs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tvksacta.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ilhhyzeo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oovzldkh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhptgpfg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qfpqloxt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mwgkovhk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mmljkvst.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bgycdsnk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3exesrcip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uixlnggn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dpitpkqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3woabfncx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zqjqsnqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egzytpgp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ievstpht.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kfjugwej.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sdxmuktw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3frpcopvi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3soveubsl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ibuplnaf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qylfihis.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3firzfjtq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kyewpopy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ufdvrrxr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3udulryfw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cmgohpdc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eormwxsk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jdpakvje.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3swhesjeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3spbvswvs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rctbngsn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flsjwdpn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rcizfaqo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rbgkjbdf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zcxntvqv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rrcomvtc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mvlbfpzt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bhpdevnd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fnxbhkbv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dbjnsogw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vhpvypbp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3knlybzof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wwcyqyve.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmpuwhmz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwgivnpc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bgdnvoew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3anjemkjy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3reuqwnnr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smikxvsl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qhjynmkp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vwxnrcro.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bcqnkucd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xoqdrkkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldgkmscn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wouynolx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpkynfhk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ydtselov.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lfptfwvu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fxxwnioy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bmmswiyf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yxupqtwt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfqnxuyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dywmguch.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfbjutlv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbivcokw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxnvpmom.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xpxllupg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aqwhptju.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axeizxzz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bymsoelc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3snrsjnnd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tpvlpjfl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lwoobpus.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxocaef.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxcfyd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zbozvjga.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nmdcbbrf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qktrniar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jkrjhxvt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3feiabika.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bzcqjmpa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3mhobjqkk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jfuczthc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvfjupuz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xedyoyeh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3amnbpoun.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3untdkeqo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3llfoyzrq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jxidwrvv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3aggfebob.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3enusjpcs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3avruckcw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oujmianu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ciydnhrf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apchldvh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhmovvyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igtexnao.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lwuczlnt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xkxqcbdn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuvfgpbj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzzxty.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrmxaaga.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igotsqag.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygloqimr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3teidzkbf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwukmxzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnwnlwij.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fabjxsif.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyemqqrm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sotgwoty.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3itjbkgzn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orswdyfh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xfbxjusl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zhxqppmh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3snlymrfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bpwlzdch.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3doegwenq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jmvgtbyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kholhbct.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mdpuzmak.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtuuvagj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifwicxvq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fjfxmkzj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kkrxpxmb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ljukmydr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3odmfntfi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ooswszyh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wushlqfj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zrslqghl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtuiykgc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qqvlsvwc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iwaivhya.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wdrkcibh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3biwcqwhw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ekierrls.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwqjkbp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rmcvzkim.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tcmcedno.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnxyauhq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebdnkjlf.html


<!-- 参考信息 -->