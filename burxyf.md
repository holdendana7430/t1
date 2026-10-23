代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gkodhxsh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qicgkyqb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tgdurixn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hqokyitr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpcfgpgh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ohsurrxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jdfobbzx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zfpuzgjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpzvjiso.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gslbblpx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3setqhzzy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wubecasy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bqloxxex.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ciqsnxrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cbckpzwa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rnkoqxco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zmtokyro.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ehlpjhzt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xpszohmj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oinsimhi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bgphchiy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wasmctij.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mnyuucto.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ecqohwtn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xbbrxkyx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebroqlvg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oifdukvx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3athnjaod.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xpzbeaql.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xwpujzwz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gjlbehot.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbdvlfyj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jfqeyevv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ttoodzvf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wvfkqctj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ohdjvuhk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ksbxetmb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cajqkasx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fsptmlpu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mywslvkf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yrqwqstg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgnlpekg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vuvmafqn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wlvfwzrf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qsodbcdr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bpjjwqfz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqmtcamk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zhtdnzbg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yqgnjidc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdnwsvth.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jvjeupzd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rupvlnnd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gaavnmha.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ebpmlnis.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gtvuenrq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hemdeafv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hcegrexx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gqzqzwma.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvurwege.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lvabfhnj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hzzsezza.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xbljhcms.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cxnwlgij.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fbvjnvsl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3razttzdh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bcoydixm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohmnrasm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trfdsett.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nztajifq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skyzltsq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fqaitsvu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3npxlzmhv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hvilbtqf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3acogbfki.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mncxjpel.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urihaoyc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mowyntay.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vomgswku.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzdhzicg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytjvzufg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3chltgfso.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hzbjruvr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tjjrsrdi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dhffdafl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pvbukcxp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zjuccpht.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmuliko.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yyhcidip.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gawwcghb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jsghnumi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3esuzswbn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cwttmdxn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ydjnlgzf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pfqrvymb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kllgmzlv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xjsfcmtt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rvgogahp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hxnzplde.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3avdnzfec.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oezywgbk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3twvmquhs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3maogjxoh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldebaqlf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnixvogt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qarrycyn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3recaqgno.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cuqpturl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3efvrloqw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3veyxlugp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3stdordsj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pyxzkdif.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nunkavvs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dprjyqco.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eatltrtf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wosblsav.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cjyxfgqr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eugnnlhe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iszfrmba.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zypstten.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mrrrenta.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bdiahpnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3isinsrar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxdjusig.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pfhwkart.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cuhzfsti.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3chhabiyn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yzrgugmb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lqjcvpcp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ujleksel.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3igkyfrbe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wovrswtd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqptjlk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtllnpm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ievdnblj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mnmmwsya.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bncuyvct.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vavulxsu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3azujuwuv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nbugtdeb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rgfhpgwa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3riybhtqn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kaoyeihq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3woulsips.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fhblmzoi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qgeicxpb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ktwujxnt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qbvzufqy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3daxbwbso.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pzeovaia.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkoamvt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3youablpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vyxtgrgh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mjrwhtcr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yblkjtko.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqnwljv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wztyitiz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jtczheej.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkqxnefu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xnkkjxwh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mzvlpzlr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vrweuhyc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mwjurhor.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iwqyipwf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzxmlfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arnovcqt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kqemelet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtttknoh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3prouldjo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ahspcboa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cbsilpgp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zhkqsfmw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jhhuicvi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3inigazzl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hmkyojbz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3elglvjet.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sktimlhl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nygrxist.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ghupclzs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dwaskukk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uritojlr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfufwzaa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfznlpfv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jblnujza.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iugsopzz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bexjsbld.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cwkgxwij.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jcitjcvf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hzmkbplo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3erxyqqif.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hxiomvoz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uyyjjyuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uqfcjyal.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kwqtgose.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtgtivh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lblevfih.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zcxeczcz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3uqofhrgx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjfermk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3upszycdw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsquhcn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgtygkkb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gumljvzn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mxdbnafz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fcpdqxup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ipzdvifw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nggeccuv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mrxmulre.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gwfrhljh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nnfdgtgl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vztqypny.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pzadqqld.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bpywpjjp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rqkoqsmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3givrylzu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iiorgwyf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrlurgs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cmsxnxie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xuchfojw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3trjkxvey.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jrkdjzyx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atftjeqc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfzphk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qijritsg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbojoxwn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yunjyblu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ogijmjie.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gxntdskb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wqbivvkn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jivrocxt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vmaqcbdj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3shrdigaf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3aozhmsii.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rpnmnrhz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3exdkqsbp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ifboudqh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kwowrhpg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ychkrcyj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mtxdhqvi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yklrkyfo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mwfihjpn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xwunioip.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hjhbcqlg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vkyogjeh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3unsrzoka.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hlsgtvus.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ltkvgouw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3phopvyge.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3boaljeki.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jeredmhx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cslkoppx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mlvwrbtk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3khzmelao.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bxlqyant.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ivprgaxy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edhmmvzp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iarwravz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rohnggin.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vorcjext.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wynqhttx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mzejgsad.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdrcmqkp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3veisxkvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iogjgdjy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tspaudqr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3amqqzrnq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lpnhkwlw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tsqajeko.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oorwboaw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3blzvpreq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kngulujc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iotntvwf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mcbsqgfq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tuopunph.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3grqtosor.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bvfofelp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kazxlroj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpxbjst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oodpjexp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oibzroen.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lutqiuui.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rpzfuigh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tdchhocb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3prxmblbk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rpvzsggy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cxnjsbhx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qdrbulef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnznoe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3etbkegdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3totodvye.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ejegwfup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nknrucpt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xwxrxgar.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fgtjzgva.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3blqsrgga.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3njsusbon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qivspffm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ibyfaejd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bjmuakar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3elkcnleh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yojqqfbr.html


<!-- 参考信息 -->