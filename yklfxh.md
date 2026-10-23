代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lpmprcpk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yagqpiip.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qaxjvktq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rbndbvbf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tdvbaltz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jletmqph.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yrxcsdvw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zkncdalj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ypxngcmw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kvphqxnd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahewcvcf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hlobfrao.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rygkagnr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omlolsby.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mzyfcgcx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3msobitrp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rlyckmml.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ayxdyukn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbfwwpik.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cyxvssnt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hfkdooxg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pavmfbxn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wamvoimu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rlkjcizs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aeufqatp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lrphzxtg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pydigush.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qcuwxmvo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lugmwlpb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nubzrblv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zzurukln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tzvlakwj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3harrlfry.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3alyhbymb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3orqhdser.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pwljdzkf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrvkvzw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zikakyeq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ygwnqigz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mqwqnrmb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tvgqress.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lefqflhe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3huhitgwj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zocnwfox.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ncxnwfmg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tlgeekob.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wvkxksew.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvebmtwf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kmyeqhkf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ifgxsitz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vsmbuzgi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3axmnbagd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gmdsawfn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldnughcm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3omjurqfa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ysijqgkt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3iohczpke.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mdychufq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xdvjmzyj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3evoodrhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okvuendz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xstxyewe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3letvjqrb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eovdtgmj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ymnbhypb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gtyftvbt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ohyzcosj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbbrjqoh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3aynjiysw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nwzezqeh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lxiynilj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lclvgrlw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dhdxvqkf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ldwhryoc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eosdwpuy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vacxjgop.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmybuuf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bjvknhgu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtjddgs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rusjzrny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pjybzcbg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ydgohocf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xuoccrzx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3brkdhpve.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3grkquyyq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcbpdsk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3efmsuiiu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pkqkggeo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vpsqdpgg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gefakfmk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3daurhjmi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3edswymoh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qdiadmio.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qylljazl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqkolg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zzwhazgk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hrgebfhp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gsniqodf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dtsaqeha.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zogzezas.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dxobqgcv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mgqjmgmk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3awqsqcgj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zyydoqhk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmwhxca.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zumxsses.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xpdwazzi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mktnkhbk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3slsrdcdb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3krpxcrde.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wtunqlnn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nagamusa.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgszqlsa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3etrgpipu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hyysyknr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqcnpjfe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fuuyvtsg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zzduospz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lrlzftkt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3unusxabl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqefyqw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3idkumjck.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxrnfkmw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkltqkel.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3njfryjdi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cvtohlro.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3whxvvvoe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cngzasvl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3igflkugn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iesdkzqu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lsubsfic.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vasimvkk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qzjqyqgn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lliigxcw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ckjzgjep.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yjzilajv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvwznxog.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hadpootd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tyjrqqzy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3emympuza.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xrwuwtxw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3njsiaqli.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ufjwsuqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bklhioue.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fkbzowjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3roegtgeo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rkzhsunq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prkontun.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xpbalgek.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oyqvhzxt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mjxhffpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3izgyxnlr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bdktvzjm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmltjqkt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qbhikklf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ugouapad.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3boahxkho.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cogdupfv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zifhamnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wrqzdxnr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3evfznyus.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tkcsclxg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dvfqhfbx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nsmcivxm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lxaeeaxb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqbqbghs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jjtcxjtc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zgfsjmov.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kggdpkbh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sndnvktc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qhbxfubr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oooegonv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vztodmrv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmgwcvoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xyhhvtbj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fzgdvagh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3doosuobi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vqepjlko.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nheufnlw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yvinvvzo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rmiwqmer.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dpcwmohl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3nkcztnbu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wnlntrwh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zftvhihv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvbjexv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ahauyuri.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rlhypqwv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cbpdodmv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dgdwhjqk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3depzbgtg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpgzpg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qaendwfn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nhshehpq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ezaelhcn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qsafjklb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glnafhsz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gihjdetb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ffssgvga.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yduucuvm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3doigspdv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xaxmzskw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gawzunsm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vnndemtt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oofdvxuo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fccowfby.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kdbsqmha.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ctrrzyyc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zlfkpebe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ibmhfsil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jgclkstj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bezpvgve.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zhuoanac.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hzgmsezf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3umvlfnnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kzuvdpqu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gjennqax.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzeckhb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nrygyhet.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pzuqygov.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uzoswmev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwfpoig.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bptnlrka.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xggybtbs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kywqcnso.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uxbucvpw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mmjwpmxf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkdddhty.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hibhmopy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3atymcfbu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3suzyoxpu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dwlxzrfe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wmxflbti.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ayxtkdox.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yvbouqem.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vpkrqpup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xihrwntc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydsxpwrw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyoacvdm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3klyakuof.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zibmalpz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zzdnytyh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xjtnoerb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zkqmjoxb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3voinlqau.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vaddnsnk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qckcfyoe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qzmnzfpb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lnpxljqa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vwikedxe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lavqapxz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xfcefxnl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3egprzhsl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kmksjuap.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ebzqplqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lbglexzj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fsmcasmh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvwfalg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fcezntpn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oewamevo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3azrnhrhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdsdwgqu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3acpbehth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmrqxgmw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kvnbjmhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ctggrnxg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eotidmju.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3duucjsdq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gmistjym.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3emjbvmfn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sqlfqnel.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzifkmsv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihuwrhnj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ctixnocj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3okaccxlp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iuminvgq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rwonfzzu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zcwlmrbw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zhgdvhgd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3eijnomum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lrcljhau.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tessszuj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kupkunzj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nukmqgip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3khzxwssv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gqfpuzvx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kkotcwhr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wzqterxq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tvpinrwf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sbjixhjz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jihbneyn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fnhgmodf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxeirrgr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eihyopaj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ypbzujpl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jmmalfuo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3etkzdklh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wfbabrfe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3glmywvos.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3njvkivky.html


<!-- 参考信息 -->