代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufxovarc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hsbdsrbj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3sjblxbwu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3npgabmpq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzcpcki.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lktrahvz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3augokxji.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qbcfixqj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3exzabndi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3honcozyt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cmmslrvx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdgjrgl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mcraupgp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3izgopceu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3komzmmdb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xlgxpbcm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bkuomidt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gchaqpxw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohsqafsu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yxnnycsq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wolaokxt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hpcxyvsu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhuiuswr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3insahfjo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dgujfpao.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vxfnatqt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bezobqeb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3agpwtnen.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ropgskzx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rqtcermq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tjcsmmso.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hkgznvxn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyixhvno.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wnopmszp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wcrgghpp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kzcjmicx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ybdyoplj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzbhumr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nytbejph.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3axatkmle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xltncbrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vtsvxlog.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxvaopxg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qylwnyea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wuhodpvb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cplyulbk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdyljbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jrzrnpgt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ffnaqdzp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xiqiwvhl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvmrsdkw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3izxriqrk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pnwwexmv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zpriidyn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gagsllno.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zbfnevys.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3byqrutzr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ziekpsou.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cguycvyk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mkjfbikj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uzhoiejn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uzcmolas.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hspbyhna.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kauhmrgx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rkxyubkp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxirgkd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3aiiwjyge.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xsnpwoop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zagkplxx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3twnupshy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3liyhgzkm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3disousxl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pbftpahs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cafuapvz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jehyfmnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qddhyloo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lsmbfnwp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3watdqjoo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3yffbkieo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmskykjf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ysrxmsue.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vaqsoptr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rytkrpqu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zcjgfpsk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kkdlniqk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iaizbwfk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xudeilfj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmgzvgnz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3skiskjpd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3okfiqikd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dazwelqa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vzxlbsnv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kijwpfyj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uvbzuife.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkjard.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qlztitol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yjvxitwp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tvxtjfwo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcjisxi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ihavekwy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kwromkou.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nehhgnii.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iswcwxhj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3aoqdkefr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pljtzkjr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rdgtnaau.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhbozwxv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oyeslwgt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3axuwfdqg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvgzabx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nwhjtnzj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvlpofra.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcphlqji.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fntdpkfv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xywpwjqa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mtmpthbg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kogzesbk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xakokxhr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpvbykbp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mvhpkrcg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3psnggbdc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jbwpnpao.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xvpkbxwz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zczgwmol.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qjevmmzy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tcmmabfu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wikibbyy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqucfdv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adtqnddw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vifwhwxs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3obpuipek.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bgtyuqrw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ifsqffkz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xslecrjv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3meqlxzkk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xgqoqzgz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dpvdxcaa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qhnmekeq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bfcuxiws.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qstuyszm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ndmbkorq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kyzfprmq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uvmncsvh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ulomfmiw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qwvqqgwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ziitcmzi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxkeafpx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqrnhdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rymniswg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmfqlvs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xidqtrrk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uzrgwucz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xpfinglb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qgzgqqme.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3effvyxwb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wmebvwgu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nycspfgp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eoufrjgm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jnkuyjop.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3isojdkyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbgznwuc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xywacnxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpnrzncg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kcmrtnwd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vvbmaskz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dekxhswr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3twjdbtno.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vuedrgoe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kqctdcct.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3igtouqbn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gojblvav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kpoglyxc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rdemcjhe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ghmdizne.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpbderew.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iwefulve.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulydrrol.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cighvyeg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tugbpbxw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3civdgnod.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xkekabkg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hfvrmhjq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yblggclq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jggoywtt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ypniwwhv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3koasvxxg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3powhahdg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ounbgbfy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fiyykcqc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jxkvvaxs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sjwasngl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gllnircf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dkjnthmk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3exbikwyh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rhylpwrd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dafqwzwq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ekkxohie.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eudsxikj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ioygwowb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ptskoymu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mezxptyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uvpkbhdr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rykkqmdm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3izpnjqex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kteuxpge.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wnskygth.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uhnocycy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjxapzl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3cdpyazpd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3unxgwglb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3olxwmbvq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3insdouod.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjcfour.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhebwdn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tzxxqsui.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gagladha.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grfwwnxq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hnkoixjk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3osofnlgv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqoblbmw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uosakksq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fpwqgtgu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kkxgqtit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cjfawvmr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dhjqcylj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bqipmdnl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xycgfwdp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3meakjgoe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nuwhvvkq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3moxhhpgj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3woxdasho.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hecafewq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iwkojuvw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ohauxcjq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sgcrtita.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ogkmmfoy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcrczx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3axsauqrv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aauzknkx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djnirqfi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sllxisqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gxnjndas.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dxbdcsvj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjyffuoa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3eumbamrs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3binwwwdt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3esdauflq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfcoqalh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qhyewrts.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hzruxorr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rktooitz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qowxaqyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hqzolsin.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdsrepjy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jhwgdrln.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3btjtmqto.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vsoobufk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3otsjoips.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3oktvettg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xpwxfgfe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pabtolls.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tmedxaaw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zqhclahc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hpcpagzh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zmlozvqd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gbxruvox.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3feuudfkc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nhskyqme.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bebwfzai.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pdkzxekj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vlepiakn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ssmqesyq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hknieeqs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bneflzqo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mvowjtcc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3birgdtwp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ddoqarbc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gfpofgxa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aisjtnak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ucxykoyg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bytoyuyo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3aeyerxcz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kaxsvjha.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjqengn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3roplltjn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpymycm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3pcfqzwzx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dmgibhqa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qugqyebg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mebqrxnn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wexzzdaz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzqdaxg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ireaegla.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yljzwyfi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mwaqmexr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tmaajtoc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pustjpxo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ktjswdqt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ogzwazkn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3msimylrt.html


<!-- 参考信息 -->