代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gupnwhwi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wdqvlsky.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gfkqlzem.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dtdtayfy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fstrdbjg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vbgdsnmf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmqbczp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mjfuwlfa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tkqdzznd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bnezgzlp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rzxnddqi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcnlnqev.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xuugwich.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3icldnmvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fwkkdheo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3csnlnsls.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkiukflr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3izvugckb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aiwkznci.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3guzbpdde.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uqctzhnp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfckylx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oarbkacm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bvxhvxyt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3difqddyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ndayoouc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymlhhant.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3godgkphr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ovmkayaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxmnrarw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kivrkpmz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbkxukh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwcmscah.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kbyjmjug.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxwyzal.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yaxppbco.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3swcoxiab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3crxfwuir.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxzqbuch.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hutwbtbz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fwxqrxcd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqqhzi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3izpblisg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fwevwgwb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgtjvwtm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gbefgzwv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcishlc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcddiwzc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3izzucskf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ccilnzzr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pnezglkr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fzrqatps.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yksswaho.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bgwatoxg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hyspvbsf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txweibuo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oshtcgjb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ygeyngmy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nyncjldz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fzndexol.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktyhqdom.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3utpovust.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ysaytaaz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nccogjfo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dgkpvejn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bxykqdok.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnixjob.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3huzxzueu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htnowoum.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfrpnnen.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hxysvdqr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dajrdtug.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zlohnmgh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyfussvy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xbmemzqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jlkdzela.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jgamgnce.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pnieoaif.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wpgvimkv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pxrunhuz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sjzqnaob.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3iiuzctpt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyoxogq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxikayaa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3brlzbuyy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mcopfuwk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3sszwzrlk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eplssvak.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hnnzigkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xbframqv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ksnjsdxi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pyqhmlrn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kzxgmieo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwnljdth.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mtzjeave.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmpzucy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ffmxnqfr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3csdfptbu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ypumgzgi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3iyniqesx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3batjakxb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pawiobui.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bbbxiyvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3capjzgbb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jbeboqub.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vkjxuspu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oynkwmtf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hnlksyth.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vtxsyrgs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kxdcvspv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bgewaykg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhmbgcv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhlupltk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3eggkjmhd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jjxvlumy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jychlxvc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzcgnj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3elaxzyoz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lantwtfm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxvywul.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bktcnfci.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ugdjmzcw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nkzauspg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yjsnnsdw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3esfhzcrq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3asjuotpa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lhqutptt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lymoawnm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ywaytlch.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehscgfky.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpagjeew.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxopuku.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zoowqvze.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pprsqnun.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fgogjuyy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fsuiduxn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cmykgkzk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phkgpuot.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fwussdkl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gstvpzkm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3obzizkpl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zinkztto.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uvtdoood.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aliwczha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xskvibey.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eprkktwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edepraqb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yrtzwdzr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gdluqrhp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3acoaresq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3volldgux.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ehyvhftf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3folstavq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rvmbrpqd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3elqbxxtb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pffdcuaw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fxalhdbz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eurvxlmv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sjqeomei.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tyhiktat.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3soztncwg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwklmid.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdblnqc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qrpurloc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pgiagtre.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rjgkbbyx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cjtvczpl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gwdaouoy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewlatebo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nfcgoqlq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qeobveln.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3isohtbhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nmdmvfmd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hwijdhwh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hizzcxmf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yqythsju.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ggfxtlqn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3lsuscbfz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gutunkov.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rnbqqooh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfuvzrcd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3etparnch.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qghklcdf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3butmhchj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fwsxktvo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ywlweagv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3owrgikpa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hwkiuwut.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3enzakykd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bbmzcxcf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bkpviduv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3flwrcmrf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fzetrjse.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyevauiv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3twayomap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fphakdfv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcnxdyjk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fwjpxqdi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbxvnim.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kymivcbk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zetfitbv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uyfaaeoa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3otbqxvjw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nwtlrzuf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqxofjy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iixcsqtt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mvsdaxzj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bibksfip.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ttwoqpgb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rviqjkip.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pvusxfin.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pjmimfqo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mgztwppj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nuckqjgr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eacqsxst.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqyznvp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wifwqswz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lylmxzjx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ubztcsko.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bdssavsi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lylqeuge.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nstfyeoz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fhmbonsg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rwgvdbqn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nhmqqlyi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3prvowwgm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dohplpgu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwwuakmw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tpqagqhn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdrgfmxn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uulaupwh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3stlgwefx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rxyufdwc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3codaqoju.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwklbgr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pnmqkskw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lbxztagc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qazzeohv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxdihyis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uxycnzbp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfipyi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tcbmamut.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uylzunzv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3prpvrgia.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rebapcnq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xgcvisyq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qnzblcjw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jsxouooa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kxgrywqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aoxfmzdj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sgbgslns.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pacpquxc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3iejybdwr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nzieajqg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ikcywuuy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wgupzsiw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xlbpzcpg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzkmzlye.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3substklu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tijglkjm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfneacs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckchrjtf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vngsoyxe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdryurve.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xmtikqya.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dtxjjuqc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhndsqxi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hmwztvzt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3chwqmnio.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mvzpnuug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pkzcetca.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ugxvlqnn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwdncp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hqlyfvun.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3smbwdznw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ateflvri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arkvpdac.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vagtudpl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ggtluwxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ahyqmbkx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3azeyxpxw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eidxztxv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kaemrleo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3exsiftfo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ofqacwwy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ckkcxbek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxfevwo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kmxqidab.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhmakc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vcwkctau.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ltvazmkv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ltmhgabd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xqrizkss.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ayyimeqq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypaymrbm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vysaicok.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pvebikox.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3twwujrqn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qgpuojux.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ygempffu.html


<!-- 参考信息 -->