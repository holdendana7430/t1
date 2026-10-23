代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lucpvtal.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfjiakvl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oyloaiaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uyevuxls.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3iurzijcf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3efczkgtq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ydxydzjl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kdvhtaed.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gukrzhlw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wmuurocb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejjbbjty.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3esgrkrzx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yqlyybhc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ctpnwwbv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwxdoeyw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlhubsfe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hwygpxsi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3iqhupejc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uxhyasyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gunnnrgi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oupdphij.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkpqlcit.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pllfynzf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqhqdqj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmwuaqv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3smekggnw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rancocru.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ytjxgofp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rnrfsvua.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ccrbwyhk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xophftem.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sfagprhm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jwysgveu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkcnovkw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzmddshg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cvqhjoph.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yfaxkrbt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhftigs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhzudzp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yfijnunu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ozzppwfa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lazierqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oihvgfaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkrufzrn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3canvuwet.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eptvkrog.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3elsxonah.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3erkggjqm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sgkjjdvs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wtaauuyd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bxirjdka.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wmwcluow.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zpckhkhp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tujadiae.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwtiwiay.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpjnaqum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fyrsahdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmtwcbln.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvtuvqt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wzhojbmv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ydfefqxt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ktfbnduj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ayoxjmxr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlyiypz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfyhppqf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqoblpoy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixggrkef.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aonegjky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkyvdtb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qtcijyvd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wucsszry.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3isbyvdnl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dlazfmum.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3boftslug.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3grozfgiz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lhswkjey.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ilucjfum.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wqagyfsx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hymztlol.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcdbjesp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qpvfxzqd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3limgvdrw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wqmfbmmq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fnqcxqlu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lmlefzad.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ebufansl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eiaalgzs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3icsoovbz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jtsduulb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xkrgyfhy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ioekovah.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwhlccc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ywpiwnkg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bxkxxclw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kwbuzpku.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yldygcrj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dxluwhmf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xdbgdxuh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xvjeypmx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tuwjimvh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cccqsdoz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgahlwo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqtxkulq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmoelzti.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylurfrir.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xxkvvpaw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3keukjgju.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3esseztla.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtwgleim.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wyneumpa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aixdpodh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wpseysqx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xcptwgry.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3emziepka.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3opmavsmu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rrxiszec.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vdhkrfmn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwquffr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nnyyigcz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ouaikylb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3amgggutz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sqadqcir.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mhgbtjda.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lghirasp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dztminzq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3csgragdf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxzoggs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oiriowwn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jmokoabv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sdvlnksn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tjlozgie.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrhhgqc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lqupxfpu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3spjrqftl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zzlzyfre.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fpherfri.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3baeqmots.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lmhbgaxg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3feizyvij.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fxrhhfbo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ilyguitl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3orhkerxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dotauprk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3babqmqyo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zxxnwbhn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtdwzviy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qrkfcqep.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3smkqeyln.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jorvcohk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ivbefqtz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3binactrf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrenrtrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tizmqhuq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3etvrqwzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkhgjkuy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mhsdxjzr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3piyhnznq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yvlxzjaw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dmdiqgop.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mohpzhjx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rascvgqr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mviiikvn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qbunuijv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qvobvwjb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xwmtovgb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mwcbpvsj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrwestua.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ismrmtfg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hqhqkznl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhtreun.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qdpuoxgz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3koijqgwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wagjlqpi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gtgeaife.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ijhkdezv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3miemnuwt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zjigkgtl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ocnivhwx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iozjzcxj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wzdamqck.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tscxsvhz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3umawztmb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3atbpfizw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kojcyhvp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zlnmbazx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vusoctbt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3evcwadwb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cstbpsem.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3srxbgzuj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vtbaivlx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lajzzgiv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nunqokyk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3itszbdhd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bvijmsxe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqhefqrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gztkvibp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vefnzizf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qasyqxlk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gkdcjmrc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cngibbts.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uedoxmpp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zubbxpqz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odmsxdut.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whbppcsk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kkdojzhs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lgydinke.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nxtmsbco.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uymzxxzg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iaiabomj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qjjzyyyz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3irnggluk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pphyoujo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3daqsmwmt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwutqk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3alzrplco.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxhebbf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hqbtizlw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fbsdadjl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wxvgriie.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nxlopqvc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sgppjhga.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lbgblzdz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pdpdipcs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lzkqlhgc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bisascps.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zhvudoxd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3whjkkqba.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fxgrqmkb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhopldyh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wghijzae.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pbnszfkj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gmxklmrb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gluilknm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3itfxirlu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tlobduev.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3evncriwx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sxwebvsa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3avlobxtw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jbkwydpk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xhojrwxd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vhpdlrst.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3npcqwubf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ucyvuskc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdnvsha.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yujbjtoq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ggtrspam.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fttafmfx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gjgtkwjf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgfwoxb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vswwsfpg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctvdizca.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gsajuigk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3olhehafy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hjixxurk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vcjwkhtm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwhieim.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kjskoajo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uihubpzm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rxydmdat.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ukpoibal.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3liuuggku.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qzscerki.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jtfmarch.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bqyzlsnm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cubexdnt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3somzjotx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kiffoqqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3shiitkdj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lfafszxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqwnlwah.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qyxpmggq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nftviszw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vcerbpzg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ezseqqru.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vpegwcao.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ekqitrod.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wiipwamf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhvjnij.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wamsidfk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mdrqvcqd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ayigjxby.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yxaffbvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqxqfud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jpelzoiz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3eeulfcqv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lortpiqb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3afeavnwc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxyikrd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3upqowlxr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbofobo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pukgstex.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ayyahbcl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rknjwmgl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mokdianc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eehtakxv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3alqaippu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3admjnjwn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fiafaizf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jumuidoz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wxxrqyqd.html


<!-- 参考信息 -->