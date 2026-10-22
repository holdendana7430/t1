代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2olcigbup.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2udcflsfo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gabhgcts.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kyamsnjz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjdlvrbg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hncnwngx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2thxauzsa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eosxxksn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bldwslzp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fzfixrdg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kjplaelx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gadtjcky.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mfmjqmij.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2teficnas.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zyhqcisk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jytnzupm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wxmwwhwg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wxnahxgu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dgqxpvec.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzffbto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2gztnijnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nxqkenme.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ahinxtkt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tqsvfapj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fzjpzavu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2svxdmcto.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oclnauqk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ogtcyidt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cucgrbcj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2omjquusf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xhspdqzn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbuilwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adetrdzt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2chsqqvtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpxmgqeq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jxfvdtau.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lqsligmy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eabgfdvb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cnzpccpv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdfymxnm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hyicakoy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dflwzcfy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hrcgtexk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pwcwmfup.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qcevpfim.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sqjbzkzz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jpxshhdj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vindkadh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlkxbau.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kphzxnnj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fguqikyu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2czkperzu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wlgnvlnj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dvffmfpb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pgyvdtey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2upihvvqy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tfcfjbhi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrrskxy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2upmupkfy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mutjzjiw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zoffrtwi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2sfjcfmfa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wssbeksn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vklpuclj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2anacupms.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tndmizvn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bltgghel.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ukecackt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kysrwltk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zyrvymuv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcfutlt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pcgryjne.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sptjdcvd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hmjdxzds.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2stqrdkkq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dtmulaks.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2onlcdaep.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kmfszaws.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbooaeb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2plrmzviu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hykskpvs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2csiemsap.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2txozpptj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bgxdhift.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cymkjsmc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kubyqpmw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gkpocppq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oupwufnr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dkcqwmgd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wnkwpevl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2idibkqsh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ujgmnghh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqnxwty.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fyvvblrd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wiohpufq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkxlbac.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2anuwefbu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrtvfiz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iqxttjvi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmpxmvh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nuvkzbcm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hcxmcsxb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xdtkdkiz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkptcdxy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qlgljhii.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2glxhdtik.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fbobbrjn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hfdrrglq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tipaphxb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dxrlcnkt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xvixwebl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vkdaealy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wfoitmlx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tbfkagiq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ukbhlkfo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pgzmprnn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vujqragb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kdfpdlnk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qsrcsmms.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlvielb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bredlcir.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sipalzol.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pflskkcg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gfhgxbpu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fabtzmjd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ffvcbcgg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iomntvls.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iopstxoj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fahtnfpb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwjruii.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2opulidqy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2slgedqet.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ufpvjnby.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hrcqzyug.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rimdwoqz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fplctxhs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pbqwslfh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpryeboj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymccrucl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xgaklora.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2urxpuzvo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bkokofhh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bedusqqm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wbfhwiqg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ehajnmfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fospfxce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vsclmdfn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzzfhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tyxywbar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fjutiowc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nknksiqn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eeirfbgi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ihacsvzi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2epmmkusl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qipcmkeh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2axpjyfgq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkvkwlgq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nybxtoxz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dskqoczz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wttbmula.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dphbfryq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oibbizzl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gedfzpsz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2iznwqkjh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mjnrablg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dsdspcpv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lwamzpul.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwpopsku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbaktuke.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rwbbdfpo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eimbhfkc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qnixeziz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cemmhexa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fpjwuejq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2indmqxvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2enamdnmb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2prsldscl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xnqvinvo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ugdqcjly.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gkxrjrac.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cjngpwbm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uuvyczyb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chjberst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cjczmrjo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbkhqdq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2njgucutx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ldqxuvdo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pxnrjvto.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vxqnnmqz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2btecwkbm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2luqitjup.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qhritdnk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zbljjnwd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjkcjqx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xlocoiqg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gjugnqil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2msphpjwx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cdsrslye.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2upwkkvcj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fesepnvt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2schyoegm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cfoqvugb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvklqlux.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wxbyafyu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ncwkofhs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fwkedxfn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vfovodzb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lnzpcjyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mhbzarnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2olzfpghf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2iblfmmrw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tsweblrb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2scemvqme.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ljortwmb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kmscxixu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ylsiclsx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qsmbybbm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cpwhojej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmnvhq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qeghdjpx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ajjyjbez.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gdoctuuj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hhdvjjye.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2brwsdghy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wryenyel.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpddvwrn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nzerqqoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vmedjksh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2huijcnxw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ojzotvyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2teisbtep.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2knifsqok.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cncjrgvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alacbtzp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rjlmzsnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzownuie.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xesfcihk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yoctyrda.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cafsilwu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wmjezyxu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jegbmrrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lvjbtjkd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lxzprssa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdyomaag.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yddkmppc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2otohvqyu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2znsqieyb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bbidsuiz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dbhbvbio.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzdfcrpf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gpemvgld.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxvxpwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bbzvanne.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjinnsg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ksmqmywo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bxwosijo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lqlyqrff.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wnanrikj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tacqwofa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mmhurxlo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nwtaztdv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ndvrleom.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wqbhtxkj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pgxexwcv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zxmoxmpz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2divijjky.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2laypkdqx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iengdfds.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2orxasvne.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dueqkwrh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nxpoztxg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qegijxer.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2sbtnjxsq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jskhxdsh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfzjtwjm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apakwbwb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qiuqsstb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dlizakyh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kyqldnfl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pythiiug.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qohgmdtc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfnefifk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywomkvlm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhshsqar.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eypmfqpo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qetmrwnf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zqqtjmtj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkwvfpb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2areyyijp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fmnpyadr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rkbunqaa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mhwznljw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2azccryit.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2enubqubo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uzsuzdhw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mjagdcsw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nvifxyur.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2japojjim.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2agzimgcf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2udnwqdhr.html


<!-- 参考信息 -->