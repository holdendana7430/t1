代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ufguvdey.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jgnbinff.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrxwfplb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzfjwpig.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2plgobekz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bdbhgjvg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lgmxphbu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pfjyaiff.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2aqsicubs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2whqoncxr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wnvtkeyt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lnabbyio.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jsohezec.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwiyimn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrqmlql.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzfbjbt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwjvvme.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtlbetb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zmdogwpf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xcjfmabe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxueqbkp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lvmlbczg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvhrmlvk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fafyetmf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qyfretnr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zmghuwge.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pygzezah.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jjqtirov.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2annfywih.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aobsgbqr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zrawlxkn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qaqjhtny.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jswzdknk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcdomrx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rjojyxnz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2oiouxugs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dszkybmk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zrqtcpoo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eavxtbdk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rldqxcol.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fmyloash.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xeeafzsa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwfttyb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tgpqfyyc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cndhafuf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tcjhzrbc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nbywtjqb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tchgjvov.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xnlyacdr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nsuliveo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oepaclpg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ualwepdb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lebmquvy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lukleepy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqllepn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bwdhnoet.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sotzrhme.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2arsdzvyg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2frekzble.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yuvncgvf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2opqonihx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lvhdwyly.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2puplotrl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2omqwxqdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpnocdct.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2urelmash.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upbirehn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rdaavqtv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2evnuslqo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2flivdhpu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jxweoafc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yxtufplf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2buxrqkqz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hsoxermm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bjvrucuq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxsabvei.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hzlfpnjl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kjxyzqjf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kuvqxdsn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ppmwfrxi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bfppngnc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkhhfvt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bagmxkqi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tpnrbvgc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lefpqaxi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2haqibgld.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jrpwprwb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cyrxuoet.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2suhssesx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mbvugaai.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdkhgvsa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fofprfjl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fdbdmtwu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lnvnzudk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jvodduoc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pchqcvll.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mmcujpgj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2itngxgpe.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtbeumyu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kucqsact.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kjrqklaw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vquovpaj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mezcgxdw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ypzelhik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zyxiscfy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ckgblsxn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbqrpwam.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwtweo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jypcgxkq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nbbdoqyh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iqtudtge.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gczqlcwv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2msklrcju.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2smrjlfaa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qrfbdesg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzcifzcx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ixwscefl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnvpiivw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wjobzqpp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lqblpmiy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwdrshru.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bunsktuc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2svdorcog.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjsniaou.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pcflmcqk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2txbdymap.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zcpsrkje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2glyahngd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mzfqdkwy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fjfhhddt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2madrwgbs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2khmtifml.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2respcwfx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rnosxmni.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ywdjaubv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvatmmt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eebmphvu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lvblwxay.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrzvcyv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rwfjnbsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ogtufgmb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vecyzzoo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2maixjwvi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2esqivgxm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2woqspodf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2norbhher.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2firtmbjj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vrfdjcmp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gjrtlydf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2esbhlanl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rlsotzfe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hjzumbvy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vhqcfpdo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2whzhinrk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2znazhxsr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhdubhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ijvsqgsy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ucmhnipa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ektvtkia.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vucbbcfl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2peeqmfyb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfjfmiu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uialuffo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2buospehj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qfpuuppj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kpswfcfn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vrdpsvmj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vbyttenk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dfuaszbs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqfsaxql.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgvanqod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dvfmfwlw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pawdcfgg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mzvvwpvn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hpxfcdhk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mlzczoed.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wnecklsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljjdbzpm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tptvmdgs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxezwlm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpjwsrea.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqzbph.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ftpsykgx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sgywqjkn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wmfawihf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfrdvar.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nxowafii.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2owljebfd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2soigkkhg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2etpceqxd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tcorrlai.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2exmcubta.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oyobsjln.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dhfjtgkf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2apoltuhy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omgpjttw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mvinvdfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wlvfjcxd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2eleaqnfk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlgxcsl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pticfdjo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xivhjnkr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2bwkiagrt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2equuswbf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2honrknkf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jbyglcrz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2stadjbay.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpvfqfu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2liseqvsy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dkjxfgix.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mfcajjwq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bywvrkuh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2aawqgjwm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ughxjjwe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gukvkbcy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gpottkvq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txnhuhhr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zvmvmdtq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pmawkkxw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zhrlyrdn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cmqedkjm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jwqgweyu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2epnnocya.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hevzblae.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xorqtcoi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hhaukmgh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2huwtbewd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbhahhih.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjqnmcac.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2edbkfmrs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2edtuzobq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trnddjsn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2odjybmub.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rwmqxhlf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzfjepi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yrznlphj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2twdgmjgl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2exebigrl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2afwrhfzh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wbgwpgft.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ofnntbfc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upbztlxl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bizgxswu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rabqogne.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzhhptjc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nnbhrfen.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kczmjpba.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kitojllu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2sfwzlcfu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hdjvjfah.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zkoprozd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ydtngagy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ovdlgofq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tpicucab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2blonridk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnxdxibr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebcoqzen.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joreegcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ijapjrou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2udrjuumr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqevesfk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cfrxsuvk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vbyobqai.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urkfebwd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zkpzzvhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdyvsxwo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gguuewkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrfovtxi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2epqiivhv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rcylhvqx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lfwbonba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lfzizjtb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2juxvxdop.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aelbehoo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lbensjxa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwkfjckf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tuiatoip.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqtowlrs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kkkthujp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rcftnnoq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2asbnhxdw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuytcwxt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bwsuwcpa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2damvdzkv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2epgjzteh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vilnunuz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bcyavbke.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvjgpor.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fnsoyfvl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2woewgall.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uvbmhrer.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxuzckr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mkutqrfw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dfgyzusm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kwmimjhw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfevoell.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pnwcsgus.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ssciqbiz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2blaegicn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvetmvel.html


<!-- 参考信息 -->