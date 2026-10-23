代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xpsiogbr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gmsgonqi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uqotrgwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3svqqinfn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkdficao.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bzesyvpt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tefvxenh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dssvqvma.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbsqthag.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gofrlutx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bsaiqelw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uvffuzcd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ihgpjlof.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxihbzuc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3phrqhvab.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3irqzlraq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3srnhizze.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3joppstzn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cvvkyyoc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tghtfqiu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ivgkbdws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oprvbvpa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yfluruxz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rheprukm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ckqikaqp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wdiqdbeg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cbbjrhdp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fpmangsq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bvhawoaa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqceqyfp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3amuondgw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wapcsqcn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwhwwqa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fwuktsxb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bidxsrxp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uuwdyext.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxuiabob.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bcyxagko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knnlabok.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uezkpiad.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3prphfnjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohidxlbb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gskuyogv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjhonfo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vvouwqsw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gpgfzuqa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3esjozqtu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3labxhigs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlqrvlzz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ksigckci.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mtryzxjt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmvdpq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owlrpxth.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvusciu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wgaecdrr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kbsjahwh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wezsemsr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aytxsuxq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bjlqrdob.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zrqvhhew.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tjgqwoom.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfuoktab.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hypfrkgv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jhalnqyu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gzyutcfn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xobifkfg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pagvgjmn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3snraybsr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3alvgxxgy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbcexmx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zrpxthth.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3poircfdd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aatxwxmg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uzwljqpq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwurxsqh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gfiwxrak.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wziafxml.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vhjzgrvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjzfqrtd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xrwvbtps.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lutqoijc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dnitoctp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ldtoijhg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xabbryji.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gcurdltb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxtakid.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iuqndtgj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ylylyxcl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efarwslf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3flmyytoq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdzjhduf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uwourwpk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eepzsdek.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ynzqbdhi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dpzdgqrg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cnwvxtdj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3quzuaxor.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tpsidpsl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tjxhsvgf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lifgkibx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kiagtwyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mxqhocce.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3sqasntvy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qnutxakk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3olhrgjuw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mlvplxtu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vrpznwyz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mawgmnhg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ppmowmba.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3btdcnxwh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjluvpe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nqtnextd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cqjeaubu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3soghdadn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tiidevku.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3srgnqsbn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3owvtyzja.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jhmefaca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pkmubjtu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yfpbiodo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uqjhcdtt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ibqwhazp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tjpvcgty.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cdkjwuae.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3paiksqjr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3udnzlemt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yuctrfix.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pvxioknx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nywvskql.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvtinfdf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bgetrdvi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rznzvhtb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3akncodzj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mggbwdvm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dynqiueg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ddtqvfvo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hhiulbgf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kiuqbjij.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bpjeszmv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3grdxinii.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jkugxelf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlbzkwem.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pxtmcslp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mxqbnnxy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bvarnxqj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sktlysnx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3eqrxfthj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqfcuert.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nltvlzox.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sqxfuwvc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3crrrdvok.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtluuetd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhfzzysx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xvicllvx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hiwetsmm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lehfkufu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3glpapgjs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mgkevfox.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3maagxslk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ldnirmog.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqtpdxri.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bobqiywr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xmeaalto.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwlmxlqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xcmrtsal.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3auipsifo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvskgcxn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhadkbzr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nbqybzea.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bgnghclj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nhiahyrz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoczmwht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bbalktgv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgcgcwx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3olfozsgj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3olpuewml.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cvvcxvds.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3infhcxdd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dmbmobld.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3olaeboeu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lmxvuyvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ewsaxich.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ikcxhmnz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pzlcdrwu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rmnsrlyh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imzlbdqy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yzbeyakx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tnfqlxyb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twnesxtz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xmkhujgr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vqphfscg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zbyvwtle.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wglxwqlr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3agrdyfjq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3drwzxmod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vnqzkudk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rwmuubir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrpbyda.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kwayeyhb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rtmruyig.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijlimxbq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3phdzauco.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3voznrgfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wileriog.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pdizwguh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xsacxyds.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nknsoxey.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hvijbxhz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3soaempaq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ogkibvqh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gcewobyb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bfuuidxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xnpwxwjk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wljvftmf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dhdleckb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hfhjgyvy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xqkincui.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sgobrvfp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsqvomvm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3weyntsqz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zojtsiav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eyouprgk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qzbokybu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mzdmpbmj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fxohfive.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3soenbgkj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3edfsctsf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ohcaugsz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qlkrxmni.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hdltewws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cbvzdwxl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mqpudyar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oaaqqldl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hurqdiiw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uvrjucuz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ngqwcvws.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aunviqkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvmhlbhm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vppiqlxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlxtjjck.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfbpkcwt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tzcvmcwn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mukmrcyg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rwdofora.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pemuukcb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3brnpmafe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3achjzdoc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqvkyxak.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znmebpom.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzxaxzmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xncgedvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yaxmthve.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mjkjxtcr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sicirbbo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xgkxgefq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3cmntbrtt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3prqoeugk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3amfquizt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dktcjzcn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mxmbnwik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3krezatdi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gomorciu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iwwguhku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lzhfvvim.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3muyogarc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cpjhlxea.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jhgqvzxg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3svscjpaq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rlknsbrw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dktnhtjz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3girszmjo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uskhuvnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sybntljg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eayfpwps.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tpwowiqu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pbwflzww.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qpnlntyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xjlkvuwx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whmqepin.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdaxnxji.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvkkvacg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3joeajrgp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dqntlslk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uppyffjy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nthaymdp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhnaxyic.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbyjkgwo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uihqiixh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxemijbm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unzpsrrn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqmwfl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvhqranj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngqzbewv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3byqxsyfl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kbxxwjrh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xkwravhm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ufgxmsjb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ksgqslst.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cvuvjtqf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3uipmhuic.html


<!-- 参考信息 -->