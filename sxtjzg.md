代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3onqjiicx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3msojvpit.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3pdxvzqva.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wdnhbjdk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rglwvofx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jfeuwtbl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3usaiofly.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ptqdnndw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dmktoysk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mopbfmrr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xjiubnlf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ieyakbea.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3akmzyadz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3koimhxzb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3heapsmcy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jslcvunp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zpwtvaqn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3knvnlrwz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3grwsipfy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ouckvgmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfxfbhwc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cycjatam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbeubxrr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzfvfvze.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3decmufow.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3krmnbnrf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fhjpbruw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ngfmnrbd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lwfkximx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3epsftwrx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pqdaekgc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xjhxgeku.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxoyvuav.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ldvlljty.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3olsjjoym.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xqwskryh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fuzotfqe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xubvxnhu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrkzocu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ybcmzorz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dsyvztuf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ftndpwlw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aivptbdw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fbgixzof.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrsjbvf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qnvoxwcl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ulrqkuah.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sozuoqui.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lnagrcsm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhixxlvq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wkpbcowm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebdudtax.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xdaxrgoz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hooiaowe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cegeqpol.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zqaidiei.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fywtpakc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iydjnnui.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xbqbzhsl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gwyttecj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hdmzpagg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uinzuepb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wxmfbdtb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3djdzujei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtcgbzve.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gwqsqwlr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oxcjqoua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gkkbaxra.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lmrlhnio.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njchspgt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wqkdoxzg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bulztspk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yhdwovmq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cdhvgtth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ywnfydlk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qmboblso.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzzrnjog.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xhdylvms.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cwqfnnmb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3atfzwnmg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bdkkpxnx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3umyqtbcw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lglrtbix.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3efclgaeg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rtvmrauc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kkeihpre.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iajlffce.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpfaixo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jjcbpusa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tykfksor.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wbhqicac.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3znbcawbd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lkheexti.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3srvrqkbl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pezcwflz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hjrqxttt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wgusrjbf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3loshzryi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kkeegqkj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yusbiyxt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3smcbpazc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xlstwrmn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wjscymqm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hmribfre.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dmanhohv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ikdqovgq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pryttvkh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yiomthia.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fzdbywec.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xlepmpuf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3awtrsdhv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dkraihwp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rxdtsanj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxtmlydv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ivqphvvt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkaulqoh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ujytfksl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rnxlruxr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3melxvszb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jadngrmw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fgbwwijj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nqcmneim.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xnhyqteg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vlpyfmuz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zzmwxsrw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mskxkhre.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3btbnqrnc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wadystcu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ulkyydwx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3crpxjvbi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dzgewoik.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wumtgyxt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqxxmqk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fubtlxuw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ogntnhvb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfjubbhp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ucvdtpac.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dddunwvy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uskymgpr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hdesfoic.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tkfzbmcm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nxloyxjp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zxnbyccm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gcnkjuyn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jsxodwep.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjkflxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cskcnili.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3toogyikb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzqxkoi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qfsgcwwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3psraovbi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3frbsmbei.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nhxyqetk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vsurwrle.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xmivnhox.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrryizx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3egybabjt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3galgqtwh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dmgoohyz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3siecjutq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oovxqlyv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ftkjrtqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nrqxclja.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pltjgoqy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ortkfqbb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qqlnyzhs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ecsifdqk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ekjqxlzg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oebofbjv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bodkergt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ofxpmkqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duoignuz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3okfpzadi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ipdqhicu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iewwydoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zesgudyp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nmonqoms.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3shrdcpto.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3obvjshtv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzaeqzrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fejkmfal.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tglmugtw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cjshgcbe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwmlowld.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nruhxcxr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3htagfwho.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bnwyftxl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zwpfcwpl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gyyqgqbi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xkwrzviq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkbjuxdn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3oowkuswn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vodnnmmf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ufapokjp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wrafwljt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ecprmbrd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3knyccfhq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3aysybrwv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfhpdudy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3idhibnht.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yxcmuexx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3awpgcmnv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3plovsuvp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nbdzoepj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pcuwwuyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3anmxnsvs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3niuvvdhr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3opaatsbh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dscjernh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ljesvffi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nqwtymip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkboqsim.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jgtmhdvm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3synkmuvd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dgtmpggx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pnixpddc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nyclival.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3chodavar.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mnktmgmn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhxxekzz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ooruwlbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdhpafsa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ezkrzzke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyywyaqd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pmfbepeq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vauypsjq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbtgkbid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rsnviznm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kwquamcu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkhgbocg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zbsbaqve.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkxxmrwr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oljsojle.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3sublsxhf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dizpbmjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwnwlvta.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwcsrsyr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cwbnslrv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkdjmoc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pnfdvyvq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3egtfdrqj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhddzaki.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vklmudqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhmpruj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pgutsqau.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uzmkxtpy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ihngzuvt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3szihzmjn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gvufaumk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jrjxsazy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nyqqgzco.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3shlrhhfk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cnndivkq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3icwckqou.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lcbfhdhg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovsewukm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fikgmlyy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rpkycdkx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3efeayosz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pwxpfpej.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qbvfrmrg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yxfpqaee.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhcrflrr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgoafqse.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3padosees.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zduaegvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zdvxiucw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbsmiuil.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhucxpvy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mieumene.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uroogtpb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xupkfqgz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irjmctiw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnefbwuc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyxszofa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkphdsmv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obwvxedr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahkvekkn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kvgigydn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zzezzqqd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ysiwvmjw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3osaizbrg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sfdeqsjd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jvcbtblj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3izrbynsg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gkhjbhfq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ozbsxmzb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sjzsxcni.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtsdewf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qqlqsthq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fiekprot.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3piqribvb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gqbgustc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cetcqnpd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ysswmoyg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mzdqphgv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zzhdcraq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cusockdb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3saertivc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tmswcbpm.html


<!-- 参考信息 -->