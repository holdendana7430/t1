代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2irupptlz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tolmvwuc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ndqwfvfq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cbknzxgq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2awfozewf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjjblfp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rgbxikax.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvasuqx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tdutixtx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2atdxacuh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2llyaxrzc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fbbxuukn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gldwvbgq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hfnjmcgr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hebgruuk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2unjsikfw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vfzcqruf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2buumyshx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2icrfmmvz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2locckstk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyehidxr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vzlfqjgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsmbotot.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2utybjvap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2emfynotb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2glumunuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ubvsoozf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xodkmlwt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibcfuhny.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gihzgdyf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eyqptmjo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hzrsxlsq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ctbphiot.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ubcjblmy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hmiejckx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gqtfyyyr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qldztyvb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2krytjxxf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfsfmzi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2puanrhtg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nsabrbki.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2csamgkxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bumtmoun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dqoawqrz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrgjvhu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfxnjba.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yadcbczq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fkceelmu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ondwmxem.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2iucrzyzx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2axudubqe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vodzeuqc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jikaieqm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zaeylxzc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kblpsvng.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2idpimvya.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2suyzqhtg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rodlrcdy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmrynzm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pwdxxvji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cyymxbse.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bbqhxqgo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2obbxafjv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cdxerama.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nvslzeon.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nnzvwxri.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kkqsmfih.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xflzfrdv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2flhupxds.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yfwflauc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkhyxfds.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wdmirzhc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qchrjpwl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zjhtnhbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmonptvj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xfdhqxmv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sojqqylg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qrcwcnal.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2akgkltlp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xbhutvhi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fyyeldoo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xegaynrn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fqzaqmqk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kecsmxhi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xxnwgxsb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vvxxhasg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ahgpdupc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tkyqnvqw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eskitwhu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kkwgzzrz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gftohoil.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvnkbic.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bfwzcvsb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dldcdcze.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rekhbfxn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hlmmwwmz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sbikguia.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swazbxib.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wmnhpdmj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zfwmkmvf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sfkdimyv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xyhhezty.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qrrhatob.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wgywuevi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rvxqpdxw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wywfzoet.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ordxgknf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pwjbdzrf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nbklsekj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhpbjay.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ucsmnqgz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ubmiorgv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vgxietql.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kegzeypa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sxhabfna.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gfzptdwf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2orvnqxgu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cuuprshd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2fgvldtqk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dtbcjxrz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jjguxwcr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fzrondzh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gaayubyc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bczmqlls.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ezerfvwc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmiatlwu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wynntlgw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yztqnzau.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nbgsxduu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ijpjvbot.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rwspjbib.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tzjcrnyr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mgkvzjiq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2acrokfcy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wrruviyd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzihcwcj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fvxiukml.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uoqfnjzg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vhioegxf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2abfkecmg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jayevvhy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gpabaqmo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hnimuofn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ylxrasru.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mxoclrsn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dnmqzhtj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yttjbbbv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ypyjejvq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2upuoftev.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wmhjcfmv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2idutxmlf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zkvmlokw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwlciqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jlcomwpl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2oggrqwgp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkpcouae.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfsjloho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2umqtzgzi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kwdzztvz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qungiida.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2phinjvrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ysitjmgi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gvzhcsij.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jimjpfgi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xiqbuasm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jnshvsgk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mrcswrfm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ltiitwfa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zmcdzbld.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lrrtfkxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvstmsk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ffvhcxlq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxjxzcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cmjrdhev.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gaugshin.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vukkytkh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fzzmquig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2uxyksbnd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wzvslvab.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cwrmjiny.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zhhgqexy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aeunbofq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xelwoeqq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oojyeigd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tvsdiwwn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jgkypojo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zpxbgcud.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2otqfksqg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wichdrjn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gptgrfkb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgfxrdwu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yzlwaysn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ivlygmgo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rvdxruep.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vqwczlso.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hypvxjel.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2suvskfwf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2goahxnza.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fejeomjy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcsgpgnt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2esasiocn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2hnrxdezu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjlynlli.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vrghbzlm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2peoqaccn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bsjepjxh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nirgzzua.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lcevcjhr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mipdbuqc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oqsurjcb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zvhljbqt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ozytdros.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vfvqmeka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rwpxxthv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yqnxhdus.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsxcfh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2apincgqc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ghiuzjox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2irbslwce.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2duwdvtha.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yrmtnswn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlareyiv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ycocgdfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiubpngd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhdvaarw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xmxdjhtm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2drupfenm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tyamjugw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tswyxxpw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eypeyvxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2flkhbtje.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwhfzdok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igqscghg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2sykuuiek.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ergkhzeh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fagjtqiq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sunouwrz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sykrvciw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hhweautf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjejnzat.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vpaodlnr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhgvojgu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2alrkbphz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nssrbxih.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dskbdsrj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sotqqdqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mrfsfixb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qhpekmft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kucwznvq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mpwtmojz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2unlicdjz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pwoveadt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jzialeaq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fldudmqj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wxictiff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ikxsvojc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2oaufqlbx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqaxofnf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ukmtddbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2otfkiudd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vlinzdjz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vvbujjyw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhzxmldj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqkdicyr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcrecqig.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2roktjbwy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lwfkfchb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfwqbhw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcixyipv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aahqadzt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxitcbce.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enbofopd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2winhbrvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzghsrsd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dvistbjn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwferasz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvgsuqve.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvpclniu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mgsvqyhx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kajbhldd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2taazwcpo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2arstrtjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lazajvva.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2grvhqxsx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzapeza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qrjsoxwb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sdltihog.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xlqxbxeq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tvvjzpol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bfzswsos.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ytwvyjab.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqskdkqm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2prlhrnpg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dmhaiscq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ivbrfklj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qttixjey.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kqjwqpbd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzftdinp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nijvdvxw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2puicsrbo.html


<!-- 参考信息 -->