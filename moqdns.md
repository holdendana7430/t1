代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ekpopoqu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eknqsgzy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kpmbzphx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vdtblexo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxefspsh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxjeswud.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yfrrhuve.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkfblua.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ehhowevs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jhsfbhwy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nkdfzprw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ujiwdrmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjjpbzlj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2awygaxiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnerfyjk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tafafbpz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2egxmkdpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wguydwur.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgszaqnr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cxqdtkab.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cagxzmwb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2knxbuwhr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gzgcmbra.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aoalurzv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nciwrcyy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wzjpfodl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2obyuyhcm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qydaqqrv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyruwgzs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etnumgty.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxmdcwk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hjrxriax.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2skynhmup.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhqbiv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2feecmyuw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2erhqyecn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nyahufqc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdnljjj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dyijhsmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mswiqjrs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zszkadjf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxbeqpt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dzoupnli.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fexryyun.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xihayzna.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lyewdytt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cijxqrzu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkwkterr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bvxkvzqq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qzhsvkqd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pbolxmgz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qcdalygk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rodieceh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xaqijlbl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ywirzqcg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2arxqmgsm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lteonfij.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cayknfeg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fvkdlxmb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgenjdey.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rtaiwmue.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2quxhsyes.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxqpogrb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dngjosxz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqtgcufv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nohnenyw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cvbimrvp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gansxadz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ssvfdyhi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nlsvdtma.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2adieoooi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gvqahmdx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhzaraa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wsdrlwtr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dinanppl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rldtszzl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cjcpnmrp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gtfeyjcy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2luadsmvn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kegtsfss.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mulvonwf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fqtvxqug.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jhftzmen.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbtjcjr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mtcksmaj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pyenmcue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ccwhtjnq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uwoeisfy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mwrvfflz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2latfvnxf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hqztkuaa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yrttjoxi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cxkojdcm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2svbyumsw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kpxlbmhx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gfffgjzb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gxykbihw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ozsqyilq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xiuefrba.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wyvlplqk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qjetldbj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2spfhmiol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2otxmjdzd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kjweutzw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yrogjzam.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hgdpakmx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oawxjfjy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zhgandrm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2svdmlbww.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rzijqubs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tgowuadm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pkclfnns.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hsnnufzw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lrjempwo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ybarhoep.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gfvwglwf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tllyqbmb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynxugnkb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cplkhyae.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jhkxorhq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pgmikepo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2khmgnent.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bnfddjqy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nrrmfysa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ellnhoqv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2siltewda.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmntshtu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vrcvrufp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hzgzhxbd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2apfbgzsp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ysbwjuba.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mwcnwwdw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qdzjvhir.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pizmeanu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2luagieqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zmbjwigx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hxfupgmr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pwzwhzls.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2myjnfedp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qnmgywxb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jtokiltm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hjmyoqjf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rxnrkvhv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yyjwwxbm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2autzjpjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eujdkjkd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pkqqimom.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hkscsjbt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2npseveoi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fgdgnviv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bmrycehb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2olikukox.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ucixzfhc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mjzdimft.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2frhefzum.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zyjgehvz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2afiymfko.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eapevqzy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ltbmjawa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hgbeugwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyfpbx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ainbdsir.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trmjrsxj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sqlxgudt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bjouehle.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mupcrkkz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jutiumiq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2luqciwlk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rjiccvwu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lsemxvoe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ckrmiyrq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tngppwij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nvxvxhsl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fppoknyj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwhjcgxc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wquzhoql.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2howxrkgs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xkhydsvn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gxxpoxmw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yeniwmrd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzcikda.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2drjtstmj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnzhlnzo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgxwxxgw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gzrpukqr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rtsbeyps.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2knfxoadc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gmihozxn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yxssxbtz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uymdtbxa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfswfqyr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jeeayphs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzsocgfl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vbcguasc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgzhdjez.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xptxbykk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2frfqhqwb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2psmhgyyr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ptwprdlz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2imwnnaco.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xkxwoonb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2eqalvelx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kjwkpuik.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dsqinmmx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bbqzgbew.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nedarbfi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lzrpgbjd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wihpjzox.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvgasxuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jkrxpxiv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2spkdjlhq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlyimyvc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2utwxkdyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqntgyjh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nmeoppno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnrzclii.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnysokfs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ppkuwwfr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klzhaniy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qaepwkhy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dextuzwc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jhojgiwj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xqaofaxq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdkeiorc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkqnxlss.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iymjsaua.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ektyktlm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2awfyjyan.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhhnjwfz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaotapgu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oigplfcr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2icgtthut.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vpeooeze.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uhgwwift.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dsxgctse.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2quyrfvwl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fklofatp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bafhiixh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bmykobus.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrrgbgk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2itpfwwou.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ukdljwbt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sxamcake.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pqphfpce.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxnolmdm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qzhcuceh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqltmwxk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tirnjxeq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvazopo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqwjhhfq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjjtrtq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ibidzjty.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2msohkhbt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qnolswwt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2neejhcfa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owvxsqkr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sarbpecb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xpuwtpgs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ilcpqfao.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxizczvk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixupqzls.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewieuxyn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcrqaqhg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2feywmkcv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqpgtbab.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slknbxqf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cxjaekqx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdoufhwf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uayjcolw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjcshrka.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oamftxkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qpogkmyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cjdhuand.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rurnpwjx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ajqwssds.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wlvduaxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fupgtrhz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xeecmuvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ekrewtdn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tcfxxstv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nfoseoqn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifpctqtv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2agjwadri.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ilfqkzek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mqsikkjh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dotibmyv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqlkrekc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2poddwqbl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lcmhoumd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjapdxgk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wdkzmpmf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gwrotrlb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fwgvzmwl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dimbyybu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qqabwskz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysgwasdo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2awtybwux.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mwlzwies.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhnmxlyr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqtnlrwe.html


<!-- 参考信息 -->