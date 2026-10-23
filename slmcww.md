代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qqhahngg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uikbosxw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrenekkt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lpmfhjqa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hendoomi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcqwpjt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gckwyijm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ysrxyghu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nyigbadr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dvrzppes.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vgcjoqgf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rthcegrh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3omljrkrn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ybahyqfc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dhdtgydy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qhrhewou.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3trnzxpxa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sciscmvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tkfoytgh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtbsihq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xcexrvkp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykkmphbe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3boovpxxk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xadgeyjx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3odqhymyl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pbipnshv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3yuppnddj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gztahpbk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3odwuqilp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wsfkyuxb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ummzgeni.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afxdsdma.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jmkywxoj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ubofqirn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tcdajkxb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3plapbwui.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xtwewntn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zkuxinqd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uopywwji.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cofxpqnc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zmhvnlgd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hqklnowt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nzhqkrve.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yeakhulx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txkqtjwy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cobdqotk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cubpytrq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eqrjyjbg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oagdacnq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mzhfjsko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cynaidrm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ozjlurmt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gsbfsrzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3opeglsqr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3oxqcchxh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gcqcorub.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkhafqif.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3snhegbcg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fovkmnak.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cbxsooas.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uqktacfd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ioiovymt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ppjgnglx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3blfdrivy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pwcgdrvb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxrtzb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3knbbcycf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3akiolgxs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bfnkkbuu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wqgddqwn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3roykxqlm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vowbgcjx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ynikktjw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwoiqybs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cdmkfswm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vbwpvmgx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mzjnqwxy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3owbmpmkt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdhbftol.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3blnvolah.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wgunddhp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mphtuctv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bybmcvwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vlcdnblt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rajasxxh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xvyabuad.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fydocijf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3giirqgle.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gssrekxz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ylsnyyfy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gopgnjfs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqooxbgi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cepqbxzl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3akuvihuh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3aoyfgjay.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gprwlhgm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vuwfmlvx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dipdvket.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bxioiaau.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ofkjcaah.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mazsehxp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bliokxpk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3stbncshp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipdthlpy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ktjlrnix.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yasfnirq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhhnxcm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxyrvpr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3mvqmluxy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3sjjauloi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uodtcjyq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dilwqiad.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gbrfuqvn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kxnqenip.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tjvquxrg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcsaqzw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iwlmqvtg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hdsvmihh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tldmegbv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3spvblwrd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3peeejmga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hzsscsew.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rsudndml.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qtfowdck.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mlhcstor.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3smztrnyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uljtrtgl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bonoehsd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kxbvhqmp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sscxbfow.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tmeyonee.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bxzrhbsw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fgfrcbsu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3flweemrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfeahuql.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdpjlrc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3blwhpbxg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mzsxhmxj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mbrepjqf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kisbatfj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nojngqzc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xzqalhtp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bnoshzpv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iwyvjayx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xjmjdgah.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kpmugrin.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hsulpebn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mhagftnx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dzoscqro.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bneittuz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pahwozhi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3densmqkb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ghcvdgip.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vylxtzoi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3itpejxis.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pclzicnc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbbuxaw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3orqspgpk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rjzghvjl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3azurkxvd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfiqusl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lelaiyfk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3doraqinr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulgosurs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jinummci.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3iaecaqqf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yffvyjkv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iawqoexe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3narnrrwg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sshhavdb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3senfgmpo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yvgkdwln.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xnhblyhf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iusbqrfz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgbohynk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rfezsexz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmzsil.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzprjcao.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rwccuvrj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gqbfpwfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hndtalpk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bvbydcfl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3trfecdsz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxnlhlep.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vnatmetc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bmjqpfqc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bhlfukis.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3grvkmdwz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gtwudbef.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3utfysybg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sbzkjenw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3avyecnud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3egqpocqr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xmrnbmwg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3flxgjxud.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wnlnbnwt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3oboiotko.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3romnypcg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nnlitkak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ccgdptda.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3aibfzory.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dfexkdoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3eektouhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pghivhuz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rmujyuvq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqlncoh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3khibrhpi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hpsxvwtj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3akqxijhs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nexufech.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kgbejioj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqtosody.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3byeoqjwm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsrapko.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eaxkmvpt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mameqaow.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bsvfhuzr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vcutledh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tjhfgniw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tyckvxab.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gptnfpex.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ymttvyrl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jemxfnyo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hlgyrtng.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3epxmamgz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mglpenam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhbqijnl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fpgshlhy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3axezsxxo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wuntmwsi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gblwmdjz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bbnidosy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3osnjywpi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rxodmzka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qfakekph.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ntwrobht.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uzoonxmv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xowqanfu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zpeldizg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hiqpttig.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vpkujejl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3omtflget.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hizxblua.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sblldead.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eltztobr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikoawnkj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nbxiitjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivrrgleg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kiyykixs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ftkxpidi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejaehjig.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3voyuiwfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kkqfemzr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkxxmqdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wyqootyo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqnlvzwa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vlyctfhx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3liiadneo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3solkfeqh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qfocyyqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fysfbzgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpphdfuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xrcdjoeb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfkzlmkd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xkmdrccf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vahmvulu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3yjxdxras.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rududojr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uyjanimd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3udeuwtwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kcypzogp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dcymzjlv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhzbsdb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yiaguptt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qxlpxvaj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3suzpwvnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3irkemfgu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3okvwdzgh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3olpdqsup.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpeviusy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pdnjhbty.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qegbiver.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3idmqpahk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3voybzsze.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dcyzitpv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tdkszepn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rejaezyy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prcyvhcy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlfauusv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pprzurqh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lgpyfkjg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xepxhgzm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngcaxrbw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cytuhfgm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmavptrv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fxwwqcyx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmzwyqcv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmhlxkum.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hmjgywqw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwrbbhsh.html


<!-- 参考信息 -->