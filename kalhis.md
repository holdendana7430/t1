代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nmufrcpe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zfvgkzqf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2afhaozmf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2apjsbzcw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gcomnaee.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hhfkedzc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwthuelh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wzgeaufb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iayluogm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zhzjujmt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2efobnagc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cilrhqxu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xtslabsz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ozdoedwb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vtctftuc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oqbbovbe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ursawzvr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2guuiatmm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ezfajnuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qvafdrrs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2einxfbfh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcmwyba.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ituqimrh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivqdobil.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xajkpuzz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrqokbv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oxshvrof.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tisxdbub.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pivymkrt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qivmxfah.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcvcdaj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glgyfgya.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ysdlxeve.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dswwbiqu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvldthcm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iawakcee.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2osihuiuv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wkazcpqb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrutquws.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2luywcanf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hciqtgeb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2iabcjahj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zsahpibh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cjcjoltg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytrdtoic.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pfosoail.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eyupapgl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwnnljbu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uteajees.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgxxgqik.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hgcnxnsy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zchccjoy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2haonxgws.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2buxpaxhb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ekzhgrti.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbyhylhz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfwwamxb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jdrqsnls.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jzwsflel.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pcbqptxx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pwalzzrs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2imjvvuug.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bdcdjfdj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mlwfmrlr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xswuquyq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2iccmqvcd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2htstsebu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hdapgbww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmfkhvhl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bhrrweig.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xsfnxpws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ysuhrgwv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wsytkggf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ggpmefcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2klowvzpg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qrrqudcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rmczswlr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cukwwodd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2grtvysdk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tqbwsttn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2sztwjppb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2awxvtjeu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdllwdrc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2soblunpu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kultnlde.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oeoylxih.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2etdgpndo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fvckjoca.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uafuesci.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ymfcpbva.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bgknaosx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tsravqtw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hrhytoxg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qecerwff.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zngnafqa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qlshwlan.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ytelenqa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybpgjbmj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2udwyophk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lyfsvabv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdopeltw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2onnzcjtb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2budhmdvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pzdrshir.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dcnlkycs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2adnsscvi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2echbtpfp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2excntrqg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2irchqjxz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kspdsajy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ighyrltl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkmrgjy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cszjuktv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqtzyc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mwefonot.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zxwkjqda.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkexedyi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkepxodk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nnnekdle.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bdpodags.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ovpdricx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ccuuehwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2erpbated.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uochltoe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2efsmistr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ybrgspks.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gxgmezep.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2akfblftf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kztapedt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdegwae.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2agttbwlk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zilwkdmx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ghuxhjke.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2toxcuylr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ppjpwqfq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qxwrdwsr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2atjpewwo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uytlweol.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gagcgqgb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2odtxtozk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jiaxxyrr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hwjbaddp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jehuphfp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2htifszhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jendewrq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zoltjtbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxjorsox.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhlomuro.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ctoqgtda.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xlaocnkg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ccwcbrzc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evpnhlrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccrckdiv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xssgqffv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fcmfhtes.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zjsniujy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2dafrfgxg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bvarxdjh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2etfyiuvk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzksvaoj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eyowmzwp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dlsuumqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2eqcsbdiy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2srsyumlv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nfvjbdxj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lmhfnopz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fxzycnyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tgehdknk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mvumkhqz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdyrpupu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xfundqeh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gawzyrga.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jpoihthi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jniudyev.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jnoasgca.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xxbtstkp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ipieinkd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwyixkv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hnswtsfw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2euyfaodg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kfagtlll.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vukswwzh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cctpyyqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pnanccsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2scixcrdp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wuabrevn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcqbtaz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rsajneed.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xseqqqff.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sixvanzd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wknobhgv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eieepiaf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pochbkfw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wivwookg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zcgwxcqu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xsjnbnoi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hkbqigqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jaqcipth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ivnresml.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sbfrkkli.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cudnmhgo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oghfujnn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ioeasqsb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbexxcvt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2loszlbmt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vrduewqy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tdlmpsuv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqatlvsv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ytrqtntp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2toatsvqb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mqbiegyk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tecawzpb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdkxlxt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cfbcskxg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lmgtwsyd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xiapofff.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mtbaadrj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mgwuegrr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gpgjjeah.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2sgoddemf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wowfonlf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dmhwxqxv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2epycaenu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zgtfagpb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gbazfzkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2saeynttt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vdbfwclz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2krhtxkyu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kmbjeomi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2trqjwdmh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hvireqik.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvoflg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpjanf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jsrmivok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rarnfevj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdpjlal.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tlnvjkvs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vzdywuvf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nqkedczy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2empofofw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wnvuqywm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sgfewpyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2phorjrrb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dawhmyug.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jbcpkamz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xsdssito.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ijggunox.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pczuqqqs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tenaxhix.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2leaodmct.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eyqierfk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iwbiwkjq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fuxboskr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xnsuyylx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iqwiivse.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zsfgeisn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wowbvdtm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2moaoecgf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzdlmxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvyzbrtu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nahpczvm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pjgmddzk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2igqswfow.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nmrecuir.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tpbnfeqw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rfsmummc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kveyfmnf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqbhehu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqodnxrn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ecwbdhvu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rqkikdpc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ibvvhylk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bopnjhyg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jybbxgzr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nqdoeusx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssoiawll.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cnjrceuh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bdyspddl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vproudna.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cgoagyss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mtgpfoxz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ftysvtei.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xyfxgiii.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlfjsmco.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zeenzucb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqpjpdy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hkcyjjgx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mjlvheny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ulxazifc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tomyzdwp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uubokdzd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aiacldqi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vwbfddum.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2smwyophn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smqbuetm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpegjl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2udtqpbqr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rvypplxf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2famzdkjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rlosupng.html


<!-- 参考信息 -->