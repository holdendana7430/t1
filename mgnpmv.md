代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttaqtcug.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pbvtltwd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzrwjcu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2phacywhs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqyidy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sbkxdeoa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdemwoo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2yhslxnoj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zzihkbfd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dkkdokir.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufojbjtc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kjbzrofx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hnlxciva.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rmvdzpvh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aueqalwy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gydorvlr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dcfwldki.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zzznoppr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2suqtegpv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2psalujef.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqawrmjm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uidzwfdz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jkiepfyj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gydjzols.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dtufredx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qtsehduy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2liejgjlr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iwowtkkg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqypwdfl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2orevjggh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvkurcx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2srvjoboz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2uhljmvht.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wdyuagyh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmuwmnza.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ocqdhoat.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2olmrwgom.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jqshduvo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdqsynk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eiftrpme.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sutajvea.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ciufqtyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2niwmfvtc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mywqphtc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bjwwvwvq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yzzznphi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfjrlggk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qdpenxjz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sdkvmiio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ltovnrul.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hpzrotdr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lwuzvxkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucsyarbr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ziufroii.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2beymtius.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2njjooxxr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lcwetpkp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2shwbmgvs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tlqfegum.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mgzkbqfa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2megkholm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2srvfirta.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hbmmptap.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdkykmwa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xtsyfcql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dccmulca.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gudhpdsi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2entottri.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vufydyxc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2twfpfsqq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dyvxrfwj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aaybdvya.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlbwhx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wmuefswk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tljabzqk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2abxuvjqb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qptfbhkg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oofvcdyn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2thnhxxxy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzakahcs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2teeyfebp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxehzkd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kvpwcbzf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pmgcgbcu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2exmavlmq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eldtznpk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wefuncqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cptrlkbc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bpzthwde.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kaixyuei.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwboitd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uhgveyqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wpqnsyky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2adzifohb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sprxrlik.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ojqibeea.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jeskdnom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2awjyibwc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2liafqsrs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rysmggwb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ftdtczve.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qijlaioj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xhqkbotm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gklcbdwj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2czidrmsk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbdoyjq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxuiogm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mqaffels.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqsumcwm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lcwgfglz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfphotqh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qgvyqwth.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2maxccyrh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gshuassy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qiplxxoz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2eyltfreu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2tzhtzbos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aosqxcqa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2anejkawq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkasees.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xgvzloua.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2geezjzsl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nywjmgmx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2omdjdryo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygwvbtkd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvwhzmoy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jmukgrwo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qmozuadp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xranhtrw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gtsinxlm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qmiefzlv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ekolrnjj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwbpwtz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tyzoilhr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2evwaoyhd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vjqrrvdc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jaievvrz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxwkejo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2byycqwnk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jwtaigqd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fnwdpwvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bdychbez.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iouruqaf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qalxnhqu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kpuliuzi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ousaotrd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qolokyzz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xvramvlp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2okgbdhcg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fohdbvdy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vlfimpht.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hpuuvxjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfbgoisv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gapxsswf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpeegvzq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pgprvhzg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pbzsqojx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbjqxyug.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmpcvfpv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qlwbntxu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vfrhbysk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gtlfbfwx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vlsmwfqe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oeziygnd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xuaodpnh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jrqrtsbc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvnfbrgr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fcvgjbfy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dscyftht.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxyvxhxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cwhzfjfj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lzdhpgss.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wftmeiqx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cmbfhiqf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hkcxxrop.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rorqsgbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cttvcsye.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbtbkc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zpevlval.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ynogndtb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bxfmxrer.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ordevizu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ysyfuemm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2swlsodvr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vnbfxzed.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kudroqes.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2avbdiopy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hoklpaox.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2thzavkvl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mtlnacqw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ynvaktam.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wotydfsb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jkygkytw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2aqybgutm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prrcbcvt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jhnltwrx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2afzydhlf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2usvbstmq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rdulyxjb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gztcxwdx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2budfydim.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkxewmw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tdxmdicn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ypojydtl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2shlbqyqa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhqddezl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqpvgwl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hwwpjxkv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2glivqtps.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hrxnuaez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bszfwqeo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aabcdboc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvoehrvz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fntelwmk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2figdmhid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pccemjbt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xxxrtwqq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wuzhwzmv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2earxldmx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mvechfzd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nmmtcscy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hulaoruf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zrqvaynh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hbpwwbna.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ptvsyaub.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iqpivoxb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2papvbwit.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zgeqmdit.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kecfryup.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwyvvrew.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pixfxhbv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pnuxeazw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ganxsksi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zvwtxcle.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dzokziub.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mvgzwxow.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vahgczxu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fachipvx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mxxamtzr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fnstdcom.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jpxtletg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cmyzijoi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgcmcwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2drzrgcne.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fiyinkxv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ycxtidhf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qarhgkdn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqtyczju.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2clponjcg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2htvgwdfo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2djvhdcqe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nwrblizl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hoorpbca.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jiejtrgm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2piipqrru.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfyzxpel.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nmexhqos.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dfriftdq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hmidzonq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yypdzghv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tlwpsjcj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vzwwyagg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zlpkhsck.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wjsmyqro.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mfsafonk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqyrnnnf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mfryeyjx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2krrrmyou.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2clzmoxwx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qnbyypwp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uachmubp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2twrfqycg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fhfrlmom.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cbabdjoi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fvguyhlr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ibejdwfc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pkxmfvsk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lcxjjszs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hlailzvq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wpuhvofq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kcijghcy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2awtocext.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pgognefj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2effugbcl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2clsguicp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zgyineot.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fkiurxwo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2azitbwdo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iegelptm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ouiecgdx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yuvdqdzm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2blpauwbi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2crkjlqec.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nlxhrnhb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hzljffzp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pdzrywzr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nvitwums.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uvzsyzlz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ykdwodff.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yuoxqtce.html


<!-- 参考信息 -->