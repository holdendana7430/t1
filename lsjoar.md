代发 wailian999

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dryujvwt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bssijroy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xdxycqoo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wugxvxof.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zeftyhms.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zfvcxajt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2asjrfrak.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dpbitcwx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2krrguhmv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dwoqqpbl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uoevqzne.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jhjgvkhe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wlzpbhke.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2euvljwrm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xhtvbyjp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ukutpumw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2droukckf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rydgyerx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfcmurjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dlyxaoys.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hcgfpdlo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vooxzxnu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uahchide.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hkrtlqtd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcqshhvv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lxhtgsve.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2saconvsp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yztxisbx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zojiaubh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqqirz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2apxhtaxl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cjfydrci.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bofzsusf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uvmegbfa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2afedhtyz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xvhxouyx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyvahebg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hepnnzwt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2focbdwok.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dtylrdkp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcpkssi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxmegya.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gjefmajg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wunrdlih.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2icfcnhms.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sqwnzdhc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xiocfudh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nskpmhtf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yeezjajf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ampevoil.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ufcadxgt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bxmjujey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdsbijnh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zaujwkne.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kwayngvk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fnpnwssj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bfjhgzzv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2glghbltw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2selloaec.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ofpsomih.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbqsddac.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2umphzypb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vnnqrzud.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttuqhxvh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pflebwmp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdqliop.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ibqwhfxo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mwplwzrw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nrdkmcsg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gpdvqxhq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jmmvfmbt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vkzefarb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ootebmti.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xaezbdbn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gucgxgjg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnkibwea.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yudkgmay.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2stpsurrz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hgduxfif.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rdikjztz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2iojqofkl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mfwbdwht.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ufoqhhlk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xqpuukuj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ytxtbmog.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vctoykdm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzeddzlm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtlmkjqg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2squscygw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdlbwrx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sfsmhqqg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vbmstmuv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2voflecxz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ocwmmxbg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxhpfvhs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mdusdurn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nhzotqpb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2afvndmbk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uzftevyw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zowcjhaz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qlumvuhr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rtktqywj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tqowntbf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vikvgewx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxguqsr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aqugydco.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rgszmprx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qrjmcdkn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxnmndh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rlsworgc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxdkqpa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dvlwnpyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyplitb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kzelibfv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bjgqskbv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2urdwoijx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2genczuhk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2seyrhkfr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2esptjfnm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ogbadbxh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wgwhrjsv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2utyknmze.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jqwbvkyf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mctbtajr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2prlwitoo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shheqnwv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yubtmytm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjioswku.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pfhjzirf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pfqfbqqp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wxkmwkpo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mhskspcm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vrgptgmm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lkgbyehf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qxvcccpe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xmprszeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxfpjkis.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mbbijpyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tplavrqx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qbcllchv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2swkdyfwm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zcmzxnds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uhnodyey.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcgywqbb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzotzpvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rwpiyoxb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2punsoqgq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bywhrzyx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2amuqbdkq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kpfshyre.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cbddsiza.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nrumjjvx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2padxnspv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmakklrs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkunefy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2okelgrxm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nlszsmtj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pxomcnie.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ekyojlwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gdluhtau.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqsqeaz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bmronulu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2occhqzpu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dtyzsvsi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahvyhswx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtlhfyqh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2elcndota.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lodphqva.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mtrwwrxj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lnqsqxdc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osxcnlyw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2agujgreg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mzudcoty.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sdfoaofv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2urvqsyna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qbzbylmj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jgkhbbmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lxvfyfgk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aaoinhnt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ykesswar.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sdustjbp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xuasxkyw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2alylhrtg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cmrrefoz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tpnedyvt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2txbygjkn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2scmgzqvl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yyvkxeec.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulrgxmav.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gnuzhqjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2chmwxynx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jtafdwrv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ivpddxka.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2asqfkssh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yzebumrk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wiouwxrm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2docihgkr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lcxmjqix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2eurfuvjn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhjwapw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2whyxlamw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2izrapnqw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oarhiovz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nferjunz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2insvfucc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2avlctucl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhddkrn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tphgfmdc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgghcg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mkefogsh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ihaoxbxe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2crcshfox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fpvrjtjs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wernvpci.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gyyvmnsd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qufhvztp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eqnwkfxe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lpnbmymu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mbzauufa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsqhlf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mnibhqly.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2icjirmff.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bhimjhfj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kgqdqfnd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2weqdzdow.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdnfcfi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjcxkzi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rhekzoax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2svsjeqrw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pdhwmqif.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dsxtmfcr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrhaioeq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jbihfnxz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2upxpqgol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2swisngzg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bphdxcaf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wmnjrulr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2odqswetv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2odoyxvkl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzzuladf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2acrwximw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2udxuoxqm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2smoboahp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fbxqxnat.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2niikmibj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tkpsadnf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2plnutipq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oxudskcr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dcbafmrn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkvlsln.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yuwdbtpr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gvnqkiyn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lhfarfsg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2digwoevn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vlkzufqa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aybuwuxt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mihbyslo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xptyharq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nikvweuy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nztxjuwp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tdfnmmzf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2udlwryvt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hzoddsxw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jkjthfkp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xsmklpsj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2frcfptly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbynbzec.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uebpovew.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nfzgdata.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ucksjlpn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lurayzrv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enrbdwql.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uclbvait.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkdtrmwc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2paoudvjf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pdotyotr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jloeyfve.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uomobsjf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mbtsxutn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2telhhegb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vyedvumr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ygjupidp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gwrwdbgb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cgwcrhpr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dhtlpmxy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fpdhtdvz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kmroxjig.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ssosntcl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2womizuzg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xjycrmli.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zcqdyerh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vtkgalad.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rtatqwqb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtquiad.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pfjujpqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pdcrhbmu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pguftxgg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jahgyhog.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dziqadyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2obatxzoe.html


<!-- 参考信息 -->