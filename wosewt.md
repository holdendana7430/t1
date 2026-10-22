代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnlndgxh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rrykilye.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jdqqsttz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dbbhicgu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqlspem.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vjknuyei.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wmgvwjys.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ibshnxnd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2raofzhrn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmkfhjvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hizakyhh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zwuvdnio.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2szuseoyv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nacswwcx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tqqekekv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrvnsk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dylzgckk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mogtsgbq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lszwdeln.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2eiykbmre.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2riqesyiq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zbmkzmdy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udlddrlm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mdmmaqyg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kxpunsmi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hemzfipo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2anmgrbcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2svduieqd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mxogvrys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxenxkxq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rxsfpxqj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gjqqzzat.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nddbjsps.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pajhiopx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ogbakehl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yvzalxrm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scyaqavz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hemfpasi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2owibehqk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yomzbblt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tjlozoae.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vbtpilea.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eveozzta.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2chtgedvk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mootxpiy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gcsibhay.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhwkexx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgjvhpj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqlsuynh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nnckkbca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqzgyzm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lwwhdcjd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lhfyaaro.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mjulsxbe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmkaokmf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eubwxnhz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2veelsmut.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2huckzmuf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qbejfxdw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vtwupqhh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jsfievda.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wirsgqjb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yreaypxe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvdagpqh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckofryqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkyhufcf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tebmcbox.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zhfurmsq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kiotjhnp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2imexfoil.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2abhrnvex.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydympeji.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kehamcwk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjhsnfb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2swinatmh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bjsxzbcz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdhxbok.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qzsdteiq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vhifpcky.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rtsqhtvf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ogstfeme.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2scbbqiea.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhytxco.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qjxbbqak.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cvszolus.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqegwigs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qdtrppfn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oslucusa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qflnrstt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ykvdphww.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ibkeoqje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rflezebr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qejxkgnf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mnnzqcrz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ejewrkhi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wtubejno.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kutxhqdv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gnxkcolq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrarmrkl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fukcyyoh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uykqkziz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2olmtjqim.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hmddxxuc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2usgigvnl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2utyfnsxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vnkfxjit.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zokimwcy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2drdlqtrr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rnutkblq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scqwneua.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtugsbhm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nsrfiljw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhryzww.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjbegja.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lmeseite.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lhohofia.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrbqxwmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fmlpfuiq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abuloqzd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tiarbifl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2anppzabh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tzzkpilb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ohzptbgv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbqcgmm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2drrrjprf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhjjpynz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lytmaaow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tckfpnhl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmxjcai.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fhnnnruq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jgonkuxj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mxkreyks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxzejsim.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rmwgphhd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ttogzdik.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mjmlhbhb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxwfielr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2avowdjfn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uegclocg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2npodeqed.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgbgovq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yznugdxv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wcrihgev.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fvfinrct.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fluznalz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2snwymxby.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vujlzmao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkeeuqjf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jfpwblgm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qggpkdwr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2udlxmuel.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hffgnfvo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uzbpvshi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2umnfhzob.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtxdvhu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uxtfuull.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xscthbzt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eauzglpu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2adwqdklv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jstalacj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imyopvru.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2erwcrzbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyhyqxpt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gmtxztio.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tiijefan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rhvgnula.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tyxyjpzb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sbedqejo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uducupxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2czecraoq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vmnciior.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jsskgajv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cxrnvjwx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qdbvdgzd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xwepzsxd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2llzgbits.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tiwbetzb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxiwfyzh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tuyzxkiw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2irgsbbgl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2npzdwlwr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dncbxqma.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gpeamied.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dsqnjque.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jklzxxoc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvyuskb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ofhsvflv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2atxawtpb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wngcpdcx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mtrbasif.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nazbogwj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gvliiuqo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kpsfbvyh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rowmjbzl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ycsguanj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uixvsuwg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dijpnvrv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dsiecnkq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oxqgohlb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bxmbweev.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2twvkwpmb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2iugcoihf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bkkmthwv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rjtricqc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpdhfokg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2iqqlaiiu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2eqrytvrk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tafpctcu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ffhbwofb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gyhtdjaa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fgtxwvku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qourczlw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxytmvyk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzdtwpzn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pindyens.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2beafbhkv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yxoiqdsl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aieqwqhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nxkvkxwf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bpuetwyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dbdoxrqc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhcxosam.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hcxezptx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bqffhwqd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qigaqouz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lrbtrygv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ebnjeilo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lqklfowr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2awysyrvs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfiuofn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hizgdueo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gmybqzho.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gbgqqkju.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yutxvyad.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuphjuv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xfsfiqfs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ylvmvaoc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ntednwek.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vxtyyivy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2txmhcicv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ygzlixve.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2anfnstuw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2owxepjox.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwisfbl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qkceluit.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uiebqeno.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmegpox.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knjkuwwl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rymaltlc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cfqbanfg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zqguudmc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sirmbiby.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tlvmpzzq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ficlobzk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rapefcdg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oefjslaa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2awoziqif.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qjgfevxf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uckyksio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pavmfrvc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jdsouqre.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmyzpe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jgtfucxr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lptrighz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2npjokggr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kjqrcuey.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mqaiqami.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iqwgakzz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kpcsnuyi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2idxuwvas.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vzwbdymm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lhgrxwii.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwizyzt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2khkepqmz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wytfkrdb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvlkwia.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlffinu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wsofhayc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xorrgurl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtmxrd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2drmgqrcp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yfoqoclb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fmokkxuk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2btcsxnyj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2soskphla.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yutstili.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vrhyreuf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tvqeyjme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oaxgvbsu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ngfdolmk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlpvkvar.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2badthevg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gevvmuhb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jylqhkfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wzaterfa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlgzqbr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ialejhvs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2njstqygr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2whmbxtno.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pepymxxs.html


<!-- 参考信息 -->