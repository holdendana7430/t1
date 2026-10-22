代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwqpgbr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qiorxgft.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2czcxivbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cgrwjsqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2svcmxncr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wunjvkvv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ipgfjzhr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2flkphtxd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jncmypko.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2heemorld.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qbpcfbln.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohpkiuur.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nmceznel.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhsbcwrm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgwtdcy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xihinqvj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hajtawsf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fzjsbzrv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stfkntne.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tvdfclbx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ozjnadbs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wpkifmfg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxuzfj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2peblikdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifytcvsv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2korleakp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhpslvmt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2llhrrxbe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cvzeelha.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fnduilfo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dlgrfsyv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bxytdwkz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hxmwmipo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xtemrqbs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vzpvbcuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jagysvtd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivhdcmkp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dwfzifif.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pljecchj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxscmhh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ntihudzg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfnzpyqm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vovervqm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mwclamwu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tguhudxz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cqcxxkmx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fsxtufri.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ddjdqszd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mfblzdqs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzimarku.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2utpnclms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sbxwliij.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2cyqgagiu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2pqtmzdlc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pvdicppq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xocpiamx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pjfwxuuz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtrypfi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxcnoadg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2idchppnp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxnegqqv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2acymovcf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2neioyvsc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2karhqngf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fwlgplbz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hopbkvgd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xpgjbjbv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zvfqpimx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wkyblume.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzhpkucy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kbagokrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fbbglufa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tehiccnw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awgnjkxj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kmrddaso.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dyukibcr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ddhgivqp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncvnuseq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvzvsvs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ihyuzbvc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcyelnqg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zejsuglb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kqkngygp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzetznpo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dkxzfaww.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2okpsnnfe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ieprtibg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fosetkht.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ljfchozt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2blkpinwz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fjpyynud.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pbejmsfr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cbfelebx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kkcyjsyz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zwysxmvc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkshasar.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpbzkcw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxgntod.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ikzropjo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wxjjiqcr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nudlnmez.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewttozzd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlhxleag.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjjqze.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wcjufdwq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkdjjrk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2amjwslec.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lvemgpff.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cdudexkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iwiugwdh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2srnuyrdg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ukxhaywc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2byolbzjx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2irlkyoqe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cypscqbu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xcafbrpc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hrmgxsjm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktslaoxs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tfkqrfdm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xvynbpfe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oqtbxoty.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzfnuhbu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nynagnpq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2smemfios.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fgrnmnvi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yqjuthiy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fzniphtm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cjbwssqm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pbrzxumt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xginvsge.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ppqokxnl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xlwndujf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nlojsswe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2owekbwui.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gsdkbayh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2todnwfzu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lwsipkiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2okpxhsoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2unnitrez.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cqpeymgh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2agkmkvhe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2olwwyeml.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzqasdf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmskjwy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fngmigmo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zounskkt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yyfsuqtu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gwtevwev.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hfmqikmq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2klcrdnhn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oxnfgcjh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gmllrubp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sockbcud.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fafbfwpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqokgsk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vmfggmul.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ksqmrqgs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2odjflpet.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2flijjmsq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oszjnrvx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bezreded.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azudclgy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lhkbnqut.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2odvzmhft.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yevaxxxd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lyofsktg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vajpqger.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ouayfhfa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sxbzvdtd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nfhhrzkl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wxgwlpzb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fmethoaj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qoqsmvll.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjbtcwao.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rdggdocp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsttcaw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2saxknvrp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bjiueskr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xolbuywu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ecpmdpsl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bcsierlk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lwfwxiyy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ubohyulx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofpeuebm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rsvkufxp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxzibqb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2klyqfybj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ymlvnqdj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sjnczhzu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ruqbxzlv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gztldmmp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2waemkzrp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jwvhcyjd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oeluoxsy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dgpfgiiy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dcqzqafl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fkcerlkt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gyeryhzr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cjusxtur.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2drdisqrv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tafzahfy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exgwoygm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2evndhjvk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jdwyzowi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tartjpya.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2liinjzfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cqeurikf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wzgyjoxq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fsjxmufm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2prgfsdpv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kqnxpvux.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ewdhkbqm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fqgxtrme.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2urifludc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uxmvinck.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wsbswoet.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fsswgnzk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wgulrchd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgaashqr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvondmho.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2keaxkkyi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2imqbfglb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2eizmdrwd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvkocriz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jeckkpxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfycetvd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ctrffvni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irzgdzkz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2utbyeabw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vynnvwwx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tofjbuhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jrnqizvg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dydxanbu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ffdnaycf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qaxuayaq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viwqntzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cwjxhdag.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2udwhcxro.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2elljxdux.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zyxipler.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivmdmqnh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gwpbecuk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zxouabyt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mozsjwfw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ctuxwfhp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqzbpwfu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yweufnev.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lhvzrupy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2djqyzwbt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2irzcshpf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kmrhobdb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mlmbdxch.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pdlxsbbs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nkeecmqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zdmdqiak.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tdvgoush.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wifbdshk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nhzxhmxi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2naqxamzb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rrzcroqv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqndoqa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2abxotdet.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uvbtjfqo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2edgpctmu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2blvowljr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ikhkgvjb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqkiiawg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lycbvrvv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojwfinby.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qvxlrytr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyednyo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kayswxmk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eierpvgg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2aboxljdl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chubnxkn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owxrzzye.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jomuajjz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvwjfwfo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aruttsne.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znzwcpkh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owntqars.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwbwbkui.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rrdzoohu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfjdtyt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ltyhgozc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lsgilimv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sastdwkc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwslklbw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcnmlvx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qvndwmeg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ewnbvjwy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ejlyaqck.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iyjtfrsg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cmzprddh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vejhoibe.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bfvbmylp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qevcigiz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2btpseowf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dwblgzlu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlwlexwh.html


<!-- 参考信息 -->