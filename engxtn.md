代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vwmtjkln.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eshilnpx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lrksleye.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2veyxgdod.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2acwdryhg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pntcvcab.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2onignein.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzhgqxwm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rbvqucdg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2flkzskun.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mjrayaqv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2sdhamqmq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nhgayurw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iuytqjbc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2drtmsiap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xtnaupsz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yislwpdm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oapftcyb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ootqzoss.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iejmrubo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ndhotyjh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsirfzt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fkxsvjne.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lsgvvpxa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxwpjmtd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2avdgynjc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2svtuihqj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fsecxzyp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bhdepicy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2edqsmvmb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ykqqpohe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zmrcvtaw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dxqrbmlr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psokzcbv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2baupvgju.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqodoxfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2grrhrnvl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2elhutoty.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nnkgldzh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mpugbywe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nscbunxi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qdeuutah.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ysfwwcnx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2faypagrr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ppxexqml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzezqkfq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rihslmmv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qixkdrdg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iisxsjat.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iwvfrfvg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nehspiug.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xmkhubmt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tspuxbtx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2utedboel.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2msporrpi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bjabdjxf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qlvfuqby.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdxggrs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2supexhtx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uuvkvllx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rqgrlszv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdjbewr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mpogwtjl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2waxsjknu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2clydyqnk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2btahpnqi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gxmizaux.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gigapjjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmdcgnsj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pjbwyikv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmopbkzi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dalsvjzi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zmwhzcej.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yhogcahu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rjdetmtx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yndrmjcz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2foldmntx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eiuckakr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vtcgzaye.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xkitxlmp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2edshrytx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eeyavnet.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lvwlbmom.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmntzegl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lhknuued.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tedszlgl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpftidqo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bpvdzosk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2uwqvpbol.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zvgeqelp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2crhkxena.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zmnjcysj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2atptaafb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lxnczebb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zllwohxi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2smgnpwvb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2diecaojn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dskgdtzf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2phjqutjp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hmfazmjp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hkjrwxgv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2akxnhvxr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqojczx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bkwlxhjm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hzibryzq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2esykrbsw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bigaknco.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2sobnxfzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zcifiyzm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jqxxqprn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhgiqvhs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ntccqrhn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xpodyrcn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfmupqbr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2epzqgzqh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uzkbbfwj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mktswdfp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkbkagr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvargbmf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtrory.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ukpxnpkh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2orbyhivm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wfpgxmjs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kbrolzyg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dwovfwoh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hrflovxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xjxfjowp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zybwitjp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rochzbpp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2coldelwe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pystbzcx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uciakkyj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zfddijhf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2reksrfnu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hxjuplvh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfjmqxq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jxxdqopz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kgcowapu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2scgqouqh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cirxhobm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qqjnakeb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vqxdmdhl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ftpnhqns.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xawdfznn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bthmwqzz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mzurjgay.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tdheqqsz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2efnfyqbc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bznjfuha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qjjsqfin.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oslmqfle.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lhcdqksq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lbawfshz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jznlemlj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2efsdvxqv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2acnrcybo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jmemdldu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oikchmap.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vphdnpoy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wxshxpat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lcjlzgdl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkhlbrdx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bzmwppcm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkujwing.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ktuobdow.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xpclgazo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gvcazjcg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ivgaiqpn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2murgqqsa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bllldifq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2loolabov.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2itwlqxpn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mkothunj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xdkrtfxb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iwzuuudr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2raagcmbf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pyjogqjn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fklyhvap.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dsneatbq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cvbruysc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vbnpcpyk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksngzrxs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdlgyrqy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uodqouak.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2elwcnzbf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pqklkxiz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2musfispd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pynoqrjp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vssjahzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pkyodbnb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oqyitlhd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gtrxngsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amyabfab.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mbqarxyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ofrlodmg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mltmwlsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zzyiuhiw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cfooiliv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxqktaj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uacoxxrn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uwhjsmos.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qljpjwfx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xddyxypv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jvbvejfg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2odumhztr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iolkdyya.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2admicrbe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zenfodtw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uzqctbsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vygopsqn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xbkqczet.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vvpdpsvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2folrpqxk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tzqugsgn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzxqfomh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2eanfinaf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yrwqrxuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fukcqzay.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxlmuki.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjlyxxq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2auoiqyqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cojnfiut.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qukslxvh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2shxgkrsc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2atgienqh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2poqidpid.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2exhbnedf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jlgjbcao.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eskqirju.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cpdslkna.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bqqxeutd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dwmlbrrv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jklmteqo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jyzveqze.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2utdtsezw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fvyuykny.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hkgqrjtd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ukdfkgyp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngnclvqd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axwlttdo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wphbfnpv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fdkyaezp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zfkxoxrj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rzjumiyk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lzufvtdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hruaylmn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfmapoqb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2latpvxeq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggwwaata.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tqwdgaah.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mudnpwzj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gjowywav.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2acyiivsg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wqmmpmfe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lbunbioq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhpgcfmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hlkplvel.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rzrmdbyo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tmmzlefo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ycnksxgx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2igbjdiiz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xcidqrzn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sjfldgkv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qrvodole.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2okscjylk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2osnpnccs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ukkmpmko.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2afwxwrhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ffbnutnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyfzwdst.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dxtgitbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrvznvka.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qkdoigjk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nbbdumjq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2coirnbjk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sdaxjwsx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cbzbavmt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2chtzeyao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mjzogtct.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2getgatlt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aaychxej.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwswgapv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vgajlcix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2giogbjwe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhcecsef.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okgvsrdy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dqndsrig.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2reozameb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwlkkyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rzwtqugu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dkqyaqzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lqstddlw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gardgcfo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ewaamrlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lsbdrasu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tgixxqbn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lzwrqwzx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jlefxals.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ymhcfikp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xqgumnrb.html


<!-- 参考信息 -->