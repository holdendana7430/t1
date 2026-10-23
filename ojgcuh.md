代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3imdmrekz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3butnwssg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gewnzvwk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3udbhlqno.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ixrkvpku.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3urxvpybm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfofqlql.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tpviecjo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ymauvvku.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wipagaqu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xkwdlxzx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bdrokdcy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3geoxcchy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kpvazidn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jxykwwpk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqewtnzy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxlwjso.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yovgsrmt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xrswigza.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iymtgakq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yzfsnqsx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ajzuvhde.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3czzrstrq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xkkhdedj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hufxqsmn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdhhqcn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfinulzx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhvemksm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jprfsihg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dxkvsxkw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfczqnov.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lzaisfnv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tgxrjhtg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3enguewhz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3moggdzbh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzsgphfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lklbqkmq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkjraytx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3toynkmgz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjtwozdh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qxjfekom.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jprmpwyj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkdbhowl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uneoxdkc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3scqyqtqu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3igfbslft.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yhroxzdn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ppgokczc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3blaaxvmy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hzguixry.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzvvtzz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3achuelre.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rowqgcbo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hpkkclbp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3spbabitq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3sqldizgh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3puywpoxh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3neelmwdg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3aetilmdu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wankmnhd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbejaysb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jxrxezmp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fhvytaog.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zqxyqqzf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zfhqwalm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ibebmlui.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3unnrkcvn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ttyywmqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ccarbmrz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wgulwtyw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yiivrxfw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3umiwtjbb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3toqywvfq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wbvdqcyj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3enwwaxct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vrohrhns.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3cqyihsvd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvenodhm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cylkhmdj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iiuirtut.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfffhwi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gnwssfsj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qdbnqmdn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kbtjbqfy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cypzhpdb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3aliqfpqa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpfnzxgk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cjucwsyz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aswglpdo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ltdqkean.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rirwmhat.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hnkuzqkr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dedeaqyx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mduihngx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lcshvnwj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fzofeueu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fyvvinwo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evvsaamf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sfkgfwqh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpahfkia.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhuuhbo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3musqscgh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snkbrtov.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lcpwgqku.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frkepyuu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tfedpego.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lshorllk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bgfrlybf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iyjdnnjv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lufgqfez.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jbtqgljr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qgfggljk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pvltxpyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhubhkxj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hceukrco.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ymzlguqj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bduevbvu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxfsmo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3thsvdies.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nmufmfwx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzozfit.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3brcvkvwi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3culksxlf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbhefhkc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whjhzvku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ywcpbzjr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yseywiks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dnegupmo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rjyebtfa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hfynpkcx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mpjgysek.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yuygbruy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qrxoyehy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlemayn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pwchfbao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aptvyncw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ekogzzzm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3eqetfsjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pdzqupqi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvyfqoux.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pwxeuqtx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sdoisqyp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pkdxxdyy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hikgnwgf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lpkiyomc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lotqqvxa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3trpwjoxf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gglpqykv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiziqljg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jrqworvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llytsgod.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqtxauqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qvdjtwjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxffgxgv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vronufsd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ewnujaqk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3sdorbpun.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vfghrneg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iymhjovs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jeobdpeg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqpyao.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3twvkhkyq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3asxdvjyn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gcxkdxxn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmdezap.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ednmsdvo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oekiucvo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rwhwudqk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3umeqmxif.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xnwcrgci.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yulmoftm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ofzuorur.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ugjyxbcb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfngil.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sftsarsz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rrwejjgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uiumwpmy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uccrchcj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ljfqvygq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gwjozeub.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xdzkqelo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3atzrqxwp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dhudsdwg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3frwdwvaj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hmknmvno.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gblvwrps.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ujkkroso.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yejntsjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3erbbuawk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tbvwamxv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mbcbrvme.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xixyoiqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qeahchxm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ubznnpmm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uzoypjvd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xcceawdt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ixuivjiw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qvltjvoo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vflqhvdr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ffpobsea.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwitlwxr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrkcbuik.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3leitvvlg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fsdkxlfp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3irwgoupz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3prgcpyms.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eprffhcp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3benwgdid.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3obwwawma.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hdcubdsh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jwpvjmkt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xcklfent.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3emyseeks.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vklbacwq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yudffyng.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3epzahyir.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3udraaewj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kdwiybfm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kxzcxkeh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uwqwccof.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lqiltsnq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rtmxuhky.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wtleahro.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ffbzcuaz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3gqcizkmm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qooxeaui.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oviykyty.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjiwpgg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vquzdlky.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lurglvxa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3shsjfmzk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqtkauv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xakyfjix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zfzerwza.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3iadsvypl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nyxuumsh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xohzmpih.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gotzwsml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrldpri.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hivzbohf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3urtarnqv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tmjelkbw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3apswqbos.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjwentyd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3toyshdku.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nurprxjv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pvsmjvat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gtiumsgc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3patpcqqr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3avxcqqvi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hcylhjru.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3csubljok.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3desosmyf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rknlmhjy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wfzawxhn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3krknjqgd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yuzwhazx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3scfngueu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3clncpprd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fheqzpau.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fovcbzdg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3joehucsi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3obqlvqvv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajizbwjs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzndffjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzznjmkv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3idxemlxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvvgebwj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3idmhigtj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3atrcrqbw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbavwajb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rkahmmxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lunqlkyj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3puqwhatb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3metptbuo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dgycuhzi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uhlighqo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ptkgwhwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mcsaqeja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wckfsjgy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtwsdrq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxzhzcxw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kqkzcsul.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owvesfma.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yorszdoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ukaokamz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uvmvekoo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3drxzdpkg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gwowdbmu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3esgfyfib.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cickhtqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jqkvsvxf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pfqbrkwq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ydynchgz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zqzemtdn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hgzpsmhy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wzsnwnxu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gyrrewzw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwwftgl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvdwcmt.html


<!-- 参考信息 -->