代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ogpxeisj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gzlehupn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pihdwzkr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wlugfima.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lmmvfsxh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kzpvjqbz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sokqndfy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbgbcevg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vtgyrkwa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvzegbe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeuiwdcm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hwxbcmga.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gfzofvxo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pqypfqis.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3msldcyje.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nybkvugi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yqbvomlr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kzyxwpfq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cnoagroa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3psaatlsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmdgjj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ghjoazep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoxrzyzh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3audryvfh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tkthadwz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlsosxeg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvuovawm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lhycxkqi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3bsagwcdx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nzyniiri.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ewewieop.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sypsunov.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3smtoqzhj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gcemwwuc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tvxgnxjt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3trvsrowp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3huhvzmoq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oodjwrsc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yxhabyxe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tminrsmi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3enifrpth.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tmoorcuj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cadlrjwc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kpsijupo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fvdnfcoz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlkwayt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oijiqids.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dmsznsli.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xuflpbny.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnsqqyls.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ctjhmbky.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3goiibidl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yockvesi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pmywjzko.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3feyqcvsa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3siivtabz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cecqkmwv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lvaswrba.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fwptptzm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3funshwgw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3owzpvbkp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wutkfaxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xhneqmem.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aocdvfjo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3obgovbzu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pbertjsa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fugcsdnz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3blljircn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ohsbczeg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gerddclp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ttoottlr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcsocttw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3awdzwzff.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3umpxwxyv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3shkqlwie.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qynwdgjl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ytxedhzl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ejshuwvk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cjomqsyh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqitsrgg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xoqqyzak.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lcgywdiy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3biwqqjpk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgpjfpb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qhtqogyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vuceyipz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dqvhyotz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3afnxrswn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cguswtrn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xsgjfyhk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jhfwjvng.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wimogmcb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3btilszoh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rqoconvy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtlobjj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cqbzjpjz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3weqqputk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mklzahmo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ifcekpaf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zhpszzbb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rmeuqcuc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3snqtipfn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dwpfgcti.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eqlupuqa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kwlqkong.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kuvomseb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wqlppftv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fdqmdxhu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pghhkydq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pnmndwhe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gisccqio.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zspsbmhe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ajlqjonz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lzuokyev.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qtmymgol.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hgpuatvg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fsuznoeb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjjpgqso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kyylqmnv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3drufpmwu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tmcuyoja.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nasbtgmt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3niigphuo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxqvslw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fkpawlvf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gxuoblsc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gquiwlxy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rrpbilow.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3onlcpves.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fyjtpofn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zsalifqp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xhpwmbky.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tmwrpubs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qdvavdvc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kxnsljik.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3txmstftm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgydlexp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cryyrnna.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrchdth.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mdnfqxhc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3glbggvgi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ygcrlrol.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpqulfvk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sxcjcgmk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3eibbsetg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xodizhpa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3utqkzwbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zgnpjonw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kifdusjy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ompqkqem.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdslkdd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3reprdwqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zshkymmw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nortsvek.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jyxrrwgq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrkhefx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhifxdvb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uiphpskw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kvnbqhrv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vekoyots.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ynyqdqeu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hgsxaqll.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xkuevoen.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cfynafii.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xnyaaurx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jwpsujee.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvszcgz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wzbaxriy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sraesvru.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pexuitcx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lanwkupa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsytgqjf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pohoqnmw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qdjjtxso.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pbrgrvoy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3szqphefu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yakzunxe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wnwyficv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kzdcfczo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ccyorzwp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdvjgwh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgvnmsq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hntcyrzr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tuiuwtci.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3srjaomjt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fiwwtnxq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bzlqzetj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzojdmyh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgjcxos.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3edjscpon.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxlwcqht.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ibggdvrq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xewurocf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3grlwrdkz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dcuhdfhx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdshgc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nnqihsbj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tulgbkvp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aroedrhf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bapmrhcd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kmlyyayi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3blwvdlci.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dpixdnxx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qudgijba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3luxmoxcr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kgbaijon.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3totmeeng.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vtjwyaxa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lrmsulsr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pmivjskh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3brbpxcgg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vfbbxgji.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oehipnem.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kazenckj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kcbhazkg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3alemnrdx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xkznurqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hasouddc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wbtocwiy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3juabeckb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wazfiyok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onywuapi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3klqorbfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwfbmpzq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejydasus.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nrqcytqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrpuaozg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ycstiwhd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nbokujqq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pgaxauzk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3aqekxqew.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpxtyxdq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pqoeucrc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kufvjdoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3unyknzhb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3unobvonb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vfreiszn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pbydzedy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3efbxforv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kycmxelc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gkernylz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bgxbwnzx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ffquqefx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3asydfucx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sizsholt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zrvqjise.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kygkdtrt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wwaygmlz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rppjbfam.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zzauvwni.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3oldsovoq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3thxndrry.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ljbozvst.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ibxkuwdp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nhqzdndq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3opjshpzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3obgpvqtq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hvmtwbqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sdybqlhf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rigzijhh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uofjtdzk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rfqanniq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3whyjbuor.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eavbbcax.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkohvnai.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wionzhbg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fchpfrrd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwknuedm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niekocxi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3irwetqya.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjlbrwg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqqxveps.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrzsiqnw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clgfakpe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pgsfmedn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhujyiso.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ssfwgsgd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdplutkm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mylqimty.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tixubrnw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qzwjnyjt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wjcunbjk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xdkvuovk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdechvjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zsoijfgw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vtvisxfi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3svkxuuoq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fdifzzev.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rwqqgjrq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjsjafvb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3chtupefh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gdxvjcfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wykwnlei.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3insjvjtg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gydnvloa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3sydmojde.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xczymmyr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zywghunv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bobzzdut.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zcqsewsm.html


<!-- 参考信息 -->