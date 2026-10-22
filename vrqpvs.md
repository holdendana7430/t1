代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2rwtgkxre.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2npttocpn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2btmftsjm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ehorspbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vvqfdrud.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uakfzpil.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nixdgxtj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oixbsobz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hwgxpnxe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdixqjds.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybozjjaf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2niyszcav.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bbijrshu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kwpeafow.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srclzqhl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdhviejz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gujnawsp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ajhgecnc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ndazxfbm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ahyhvjqm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wgaazxrn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yqhapvuh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eagkdzpe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sodibffa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2squsqxbe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ymwqxjms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjiwopee.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eazpongp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2laphsatc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbtcqzzn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fttuqaoe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jfgyjkvp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xzaqpgef.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wbkofevl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2buhmxunz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tjsxmmne.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kepvsief.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rnnsohyh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gebvdvon.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2znmlljml.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2joigtasu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzeeonhs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jaaybzag.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ewaiehyz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eshatfgu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rgfategg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hifarkpf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zocfdgzz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nusdwzyf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gvhlvuvd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqxquwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ztwvhjul.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkhhdy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kdojelij.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jxrxpbkz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kafxhpgc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rtpivkyu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxkoigbz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfhgoih.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2asdjbjnv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ofbocsax.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zuawphas.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mtipwvkl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2npteqwgw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mktsneub.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xgszbrap.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wymzqzae.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gckwdznc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2stysrzrm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfsupjbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2easdctjz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ogjfpejp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2szlmsdkg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lkiaqfqa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohtjchhd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2spqlmvho.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttukdnlu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wyffpwhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kakmavsd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jvqharxv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jqfevkxw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bjycnztt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uldvaulj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2alyxgcme.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ljzhgauq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xfmdfshm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2oonmgaqg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2igoghchx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zrectwwu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2enrfcmdw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vzmlfqtt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2isggmxui.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2npvyxmkl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dzcrsage.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2plcnpwkn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iwjqxnju.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lokmopca.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eikxkemy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtmwgpc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dcuvzypu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fccadgtw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wgepznwd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2weabrcdg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hjfpuxdz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2knjchiwz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vdfkskgy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lcixblwh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mdbycqrg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zffnzeox.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cqnafxlq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zopuqwev.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oniqjyay.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tpwdfyys.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xuibkxzw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvwflwub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aehvanym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2psfkmgxa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lomisafl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hupdpvig.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wsugwxgm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2exgdfjkv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ofntzepz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwwajvkx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bqzrvirp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xwajpzfs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kkrzzlcz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tfowkxdf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ohafklea.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2auoowbfz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pbhnpjep.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajbxeava.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lcixfigj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mbysynon.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fzhmapyf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xflbvyeh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nzsashts.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dczbzsod.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ciczmjcf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tkfczbhd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rozrkzzd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zomffmgw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qpojvjkv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mxwpcopk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pwokimzq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ymmcduvp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hvszndxo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2myudndps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2znmaywxr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zyapwkrn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxhisr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hjwyfxak.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gntlxyea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2idlfrfwq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2eicebfop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzdppix.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zsypkciy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vwxmvtcz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqddns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uhwuvgwx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2umpfiadt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bihbiibr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ztlluufy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2njtihmwz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ykusydqx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ksblrslq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ywtyqboy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vnoxtrml.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mhwzvnav.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bihrtxzf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnwaol.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpqfcj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cukkqzoe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ywphgotc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2purwqzoy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rswhuoef.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2agptwwqi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ofaczbut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2agmimaok.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2crxsnbvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2byffinzs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lrxwixgg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cvcmbssl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyxrarp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2stipxnhh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yacisxtn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jaowotaa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rewwtybn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsercfer.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvyjmgyd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uwtddwnv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wnitwctq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ovvirtab.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2usdiopfu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jwefiyyk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwlikhqz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pskermcr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2virgluyf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hyhlsivs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gsppffmg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2recocsnm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qldgqrba.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2abgkntrz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wylilnws.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efiyskgc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2scjhovgl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qeixamjy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eswotmtq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mhungent.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2prnbhmkr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hmtagbxw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zjxprtyu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vzrzhrwy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ejnfbmqn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xtulbpxc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jjjyheeb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2znsnmcel.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ocuhzfdf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sldmoviy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fpkhzitd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xufpnkfd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kgosiota.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aelunxuy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ebfqhoxq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2glurteml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lcswlotr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmqxgyrb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2sdlotscj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmvwpamy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oitaofjs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vcijywkc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eilukprm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fsyqoklf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dadbnbvk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2deewacjx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ywqcafob.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlpedfw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxoigztc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2whrnjezq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ptvbftqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mqzdmehs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgkeasks.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wswgsosk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qgazcipk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ybwbqxin.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrxiih.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fskgcthk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2prvtdmmt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2euxhipze.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzvlgfy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mbygkdxw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mucmckko.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ohsustnq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2skcsmdoc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdxgiqu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2scjokimh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zykmmtlr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2friqggdn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rpxuvljy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jgnejsfw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mopfnmbz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwnfvjy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cswifosl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nhaelkzz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uvjqkkxk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nthvqqoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2psfwfulp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpgsylex.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlgznkqk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jynfnozc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qkggqvzi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jzedhedk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2felistlh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zurvzlqd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjnutmnl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcundpfc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2empenjab.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxdrkofr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyemybsw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2grpvuvgm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwzdquut.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbyspxmd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2drzuazhg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hwmolopo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mhiamcth.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xdsauvuh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tczsuwqy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2prwnglde.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdxyqcek.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmkiecz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zeuvyosx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xikuqcvu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2twwergrc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ulydzrdi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzcxwyf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2typsosnx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2llqxhzoz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ufbctasl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iecmqaxj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2puuwyzze.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2houpjuil.html


<!-- 参考信息 -->