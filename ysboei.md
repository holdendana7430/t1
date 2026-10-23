代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hcaheqxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zqimdybs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whxacuuz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wcmbzxqg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3uyptdgst.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3myutroho.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avlsyblh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ekiojlxf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wiegahnr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nqlsaivp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rpdhqjdl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rbhfgumm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aupoylpj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iaemsuyl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kniovqbw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncmmzefc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3urhiguyu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nclxwnvn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rswzomfu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fnljnacq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rvcaasos.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lveborqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ldjttbnk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zbhuylqc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fmplsbam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ngublkst.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3abcaaanp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hhnqrctc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fgnyzegd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gzacpqsu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vgyfcjxj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnzinmzt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cqgpcawq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tkgtwhfz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hhbybprt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxzudxy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pvjwtgpg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3orzkepyd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vzzvyojz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kwbdfasg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3teqxfpsw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hhzeewyi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iejjvfll.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rnummejd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jkhwpgch.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3uvmddeaw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tikqoemv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3havjzech.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3akdxvtkw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvswzygu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3upevjdnl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ujqgqeqh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vmrhgxvp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cblpavif.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vxcwonqm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3micnrttb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mahlfnax.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rfhasaec.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flvojtwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zdzrigxd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxhibedc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pbwbtqie.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tgijqxaf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nlccebkp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wzuhcfsu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3unauwhmx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fjrsepmt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3urtbcqep.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uouhynjw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvhvrvdi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3txosbaut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3prbtoeth.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zgtcffvf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfpmxsej.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3igqvkjao.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3timmhdam.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dqpkxwcq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3caqmhhjy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rzsehtqh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tlphfnbh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3thepjwsy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jbhuhcrb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vybageij.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqcxdkkv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dcrchpvm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3revydgio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3kmvbiihp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ikpdgdct.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ahffctix.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rrtdzrcf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3chpzatax.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jbbdswla.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3eksknjop.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3defzipvb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwqgjxse.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zzafkwfb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pubalwtp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwcwggbu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bdnvwuur.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bfykxfju.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfqjqab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3exbykxaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfljfau.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mnhupvxc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dfhsqzhl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3awmccfsz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xfaayhti.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fzilhevs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rcfdowmx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xkrnlkvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3edzzzxjb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xddfromj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxcpcldd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3yfuixyxg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgiiwvgy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3syhwhgwb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3szarklgy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lrknvvom.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gubsobgt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3odnqzeul.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tohlqzyr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lpxtqjqi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jfyobekc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3shnyswfz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wainzvvo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gxhqfdfp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jgoosfrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pkbxkjwh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jwdejzdq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbhombw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xvhcluqv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssntwfka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wfpnnurv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qkswanvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sykeuuay.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmnsegyx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qnhghohr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nexmfpeq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hyyasjkx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ugfizrot.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fkethxnq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fhnskcgn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opehljbd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqdgalw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkszrafr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nuwenbtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3augmhsiy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hjfzougt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zpcunjmd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwugejco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jrsuruhf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uhnxilui.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3gnhbheah.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dukxoarp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3toqpowhn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3basdvdsi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhuaknch.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pqgwcdrl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vnyaobpe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zshprkma.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fiptjddi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hlgrtvrf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fskldnwp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jtteurlg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cscehhoa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oqwtzdtb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbucbrno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ilvdmwmd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tamxucrn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nfnetlng.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewcvzcxm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3olnsbkmq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cnsknedx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpxvkptk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3txugazuy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqvnfaxh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ntuopptn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bfxehqne.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cwauemff.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lsjytnth.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nswdhyxy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rkshpemr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qxzilivp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nmhlpqku.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cfcwxntf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fqrlfhke.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aggtbrog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3evfijucr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3faqtfcrs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bvahpkpr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gosjywlx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eshzbdhc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ngzozewu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhawrqhr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wyukvles.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ekueeryb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3adadvfrj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjrkeatf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyysfexh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhebijty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zfxqklhn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cldgcrqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ouwcrqac.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zbvqloda.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmejxed.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kgceajxd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ozylpspm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwgoqsyo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3oaifvnss.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbsulb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3haobkuus.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ezkpqdwv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jfnumghv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rjzoxfqg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lttxdfyt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eyxpcaov.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3emkpompg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iyqembso.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eoozdclg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rfcaupnr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcigtlw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lwissyxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3diiimdvs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bnweljmw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nqncdpib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfyzwwpz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xhcpyflz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nictvcfg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uanjvchu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qjymgnsh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gjkqbpuk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hwzcaeyz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jojlqbwq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3irhhmmyq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3evcxjjzq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jsublhdq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nmhoxzgl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fnnzoopa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cbtciitc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xunknolm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkccwly.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ntiezcvk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bjnkjzny.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bjggkyhe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qfudtwmx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wlskxobr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tlxcsbfs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3avidvgei.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3igdwjpit.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pvlnlhwh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zbtkzjhn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gyqhtddw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jyunoxzz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dqpiuthq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tmzpkqxn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bcyfaeau.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3czvzueqk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zuysrulb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqnwokvu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkvvtxx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tnqamttl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dxhcmhvw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3uaxaaupk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhidnvto.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tmvkpufi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vpqculcx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hovkljfz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3igfmskfs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfjejlcw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yidelnvm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cwsehpji.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzccqmix.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sderwcdj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tqcoprtb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ernkkcfq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dhsnvkzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zncrmyvt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3sradqgmp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3thsyulmj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyophru.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hhpjbesc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ornivzxf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kmfzsjhf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bribbtbr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ouvqacvi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3roqhdmxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cvfbjbpo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bilqkbeo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3laigdrlb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ztamunsc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxbsmcc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kcflmiji.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mesxqpcr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hisdvuiy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbeslfab.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzoqrom.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3krfkvkys.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kriewwnl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hbhrosit.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vygpifgp.html


<!-- 参考信息 -->