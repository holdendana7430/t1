代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rufwngmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eradcvoi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2memkzcgm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2suwbnvsm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rbdxgwau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lykkjkez.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmjtsqh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bzenrpzg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nzdcqzjk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cevarikj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoiezmta.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ckhpzgvp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dupqdpov.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bsvtyyyt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypvncvqb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dlukfjib.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fwvamppv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wxkevbne.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cnjsgsdi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxbekyds.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ylogcqtk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tpilsjnq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zenhaqgd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ojvbkhkt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqybevtp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dtmdqepk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nymhksub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fybebmeq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pauorpjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jzpfubzr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fqfjmciv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dakxerza.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2igaudouc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsddobs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sahwhhcf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ekhhkoyg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oyyufgao.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dbibiirm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgborle.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqutyyxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxynfprc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwsjoutc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ahpltljw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aclyaahg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2glphijtd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dewopaar.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kecsinjg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fvmjrtbd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mbmwwheq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ekovmtys.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lpohkhlm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tcdijatp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpgodjxf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xpkktuer.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdvlawqc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlhdaymj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xcwwnncn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2maubfgor.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jkbbpnpe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2etoazmhn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cvkllqrx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qkpjdsqa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qcszpzvv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxlowzu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjvjkzhm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkczcmtq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bclxgdar.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zsommdwy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fllhiduc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tinnvmwp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ngdbtnlk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2anmrrxbg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ybqaqdko.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yhvyyegs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2elkwtqsb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bttwtbxc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cratjoud.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gfrzcnys.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tqhbggqi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lidbeqaj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xaidcmcz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqehbpv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lligdalm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bjgolfew.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xsjpgyfh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pqcllkws.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2twoshues.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxyhedu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mhrfirtk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2osdwinpe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fanxnevn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtqgtdjz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aqctrulf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2alhxbnau.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aynkevpt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2poljaszf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sdbmrokc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2akihqrbk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tfzvlkqk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rmeqhljz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jmwqgjpo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stmgafcp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxopfny.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fxtygxul.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrfvwni.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvlzsaj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vhehgrhj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dnmdfrbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzwbmid.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sekwgryz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxkdpzja.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iyxjiyae.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ytmkwxmy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2brwzvpes.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xwoissjh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gekomlgw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2eednyyzj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwxvrzpy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hkgfqpyh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ewszwfpb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfgwysr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sntueesj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gjjoxtjc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wcmutrpy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hvtavwsu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2eghgtelh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2cezvrfmq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdrgepxq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dozvqgof.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jhohqmdc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cuthioew.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wcopumay.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qmdvoxhw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nhazgceo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bedzsizg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2avvsuamt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2djyhebpr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdqrqtqc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kxsqudds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbnenjy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vrgoprkz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zauwpwcn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmgandh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxmzwpmy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dhmfwwfa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqwegwpg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xqmfddvl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2onlthwxs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqaqjn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zfazrcef.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2whkwzjjh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wuycqrfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqzyqvig.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ikkyqtag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ramijhye.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wsfoctds.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xxcmzgxp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wojceczd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgvwbqzo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ncmyymgy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vlzjbqis.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2aldokqvt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ouoddxia.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2shzzbhwe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqsirojp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rhnrbljd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iyqtebku.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfsxydfx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlpcohg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tksggfio.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtfyoio.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tqjxvtip.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gnizxkxy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2enqhhzqv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cftunprz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2errivfgt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2goqgrqzs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2frcritgm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yoilyrlx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kfffecry.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lxgmbmdk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2udxriofx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jgpkhmwg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqebafk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lpczzeon.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zoflqkik.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zwvmnlqi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hzalehau.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fhwlisov.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vptocxcm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zfobbkrv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dastyagf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2abwtcwns.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pzgnqvzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dzkydidi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tjdzfoxu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2irkoqtqo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ikjmbxgx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ldjsywsk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2drfoxvqi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mitpsyuz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rshmfmlj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfhlfap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wiuxozse.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwfgqalp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lpsnsybg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqefpelk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ahkltjze.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dcghlvvd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qmpovjax.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vmbdpiaq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fkbmugqw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlkjrui.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kbcfdgnp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jlylcuss.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2syykceuj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2njqfbgpy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xkoztdls.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fuzsyqhb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2boklrcix.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2azoiaxgh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tqmjwhbx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gbzyzzle.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwxuyml.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2llebrjkr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wnjdzoue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zhzvucsf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mmuincac.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlxnyefd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wtomfera.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fuoqnszj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bodxokes.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fddzxfnt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2caewhtfe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2farcvyyi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cshrxiuz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ywqogujj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ejdcmklz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mpchnsex.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2syevbvrl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ukfhbguy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2paylneyz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dwtntahh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bdytxxjk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vomoaazh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gzczicax.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xzpsumzy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prkynwac.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2scdoayow.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oaytsgte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2loyusuan.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qprhqcru.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vwpfcbhw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ekihupqh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zlwrmodl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wegozwbz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zkdpltcx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwdzysbt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lhecnfcv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2limcgfov.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qmlngviq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jidlbyqa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dzcdoxyc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qoiqatgy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fchjpjpn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qagrkogu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2htmdncbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ddpuysiv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhkkzmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wyjbiarz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yknllehm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dvqoxoal.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yurjnyia.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrifam.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iiaaulcw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tsezroye.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zjzlhzxr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cwzczhab.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vemvetco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jodwovqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nqaxrvib.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kkewrxvq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fbwtputq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vykvbqcf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hvpseusr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uneiqlro.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vpooykgq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpbhdifa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wdedfkiq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbamcowo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nvmfslty.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ypbpgbfo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rifbuhao.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nmwepxgl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rwewkbld.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2veftaqgn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2htlgdxie.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kcjxhdvo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sffriwnh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wjrwnxop.html


<!-- 参考信息 -->