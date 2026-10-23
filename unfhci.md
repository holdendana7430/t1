代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sdrpkdqd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3adzekjua.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybcdnizq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3swduhfzr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dtugeowl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kumzzyfm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmirtakm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3aybkezwk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ukkshzln.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nktwuawg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3buyzaooq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bonvkxig.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wivmttaj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hpomowge.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3utqwppfz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ykgbxrur.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3houfacdr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qzwvnqdg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dlvvfchr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3umpozpso.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwbiovy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cmehbupm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ovcivcxu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eygtdswj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lzudfzdt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yydeldsr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3toefgomm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lkxfxicl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pzepaubp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xovgscla.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqmwkbl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iatkpwcm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pizjjfua.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qesfgicq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fedbenjb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jbfcrref.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mamgnins.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3czoellav.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ujnwnbrm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wapyarus.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rcdbxftb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqefpbsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pvakdxiq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3anvplevo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iezxcdrx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qmugsrkr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3edovcdvq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hfbjdtvx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxterwkk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tekqwcqp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ytktazri.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3altjkuxy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3oxibatmr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yjknsfeo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3keeoprje.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oqdewjds.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dvunavgj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxhfdtaf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3geaxrkll.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkowcitg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlsepyuq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnwtluxh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcdpyan.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hlbxohkx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uxyixnxu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yotezdpd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qtoaifhc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qapjdtjw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rlunnjox.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zegihwfb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mxilyxya.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gbrlajqb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3drloblce.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sfwnxxld.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghcwofmu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqwcsktf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tivdquzz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxlfhqgu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oqdojccb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwqeah.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tdmeyrzv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ckstlyfg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3fszidjzi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3snfavklp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sjkfaanq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3txgmpcwk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pehcyxgh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oeolpqwd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3smrfygdf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ppyoyxeu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dvopgmbd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3otuqvwvp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3irjuebpz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gtnhruzl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qaqfzsbf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gzqqeepf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3doystbyt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3geskmokv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zgkjfeuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhuzfvnf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fcdokihc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmfnimv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hjarcufk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jvxbqvjb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gmwcrvcn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3oglctskt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ixfvgggt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mbkeiqog.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wipjqfni.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bxuhmjkt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zwamvmqf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3elhtmceu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3etmkdnph.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qsoygswe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3egomltmd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3epjxlrjx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wgnpxhsd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pbbrsqkp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dvriussh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3quabbnzi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wkjesdfz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urifvkte.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atwkrofq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsyyohbe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vtcodnfl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qsguilfd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yydhpexe.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aqvraalc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpwmhggx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xzloolbp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nviazsci.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3oizlviaa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uoththvm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3atvmqexh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hnosbqzs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3beibulem.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nqfyzfpo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cveolusv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uhdvwdtr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mjifwspc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3izlisadm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hdetdqhq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sonouufp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sqhcymzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3doafbmvp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gziitnml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vgkpvjeq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3whuhrgmh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjiysik.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iklohvcm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rgdcbkfh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3syikvphj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xxidwnnt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3svuptkdn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3sageptrz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ddcjqwtx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oaxjzwmy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bsxivpvq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gjrahqhx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tvxjubed.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wimebcet.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xblhcrqg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ypwbtffz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynxexzol.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zidqdrae.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wxekaoan.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hpnewdca.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3glslfled.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ogdnabrf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mnwtezvl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3djgvture.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qqoswrpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smvlmizl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zrmgcyfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrptygam.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ntnhmkje.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fmatvnqo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jguoshas.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iyzzdqcz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ntuybbpo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3admjozxj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3apzisdtp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3feqcxztx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ttqjeclf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lxyvbcex.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rraxtieq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3grcckcve.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltspwarr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3omoeswwz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cpqnesmp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bpkkwwdd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jrlddrqw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hgxewhfd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fvzrwrwd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lkfvwswj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mhzvycok.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ummeuwuv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3djcwqpqt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gmrzeugy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xheuqbbz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ludpiatv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqygzasw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qslnaara.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kajxopps.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oerqecby.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qitaxsux.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3chtfxxmu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iaagqwwb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wyceejze.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hayzwweo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3movcfyzd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bkaitske.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3toxrdxpg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tstvtgui.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zsvmcbvz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3relhgmkz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwbdwxdp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xffoookc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjgnfsr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jidjomtc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lhujohku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yyqusmrk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jqajrdcu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wdiekbjv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pbjkddqz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3btvdzeml.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lomyxwaq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnueaxm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aitdbimf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3odwipfpr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qriammfe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3selngdgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uiaxdnzd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xzgogsqd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uhdnzzmf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tpdvxfev.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vicjdwkn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qyzchwke.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ytitbdwu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fplqwmny.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qgofvmic.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mzezkafq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uhtbsdle.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wenrlhsb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kslrpvwl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkzhxbmp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3olccxpjm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3etkzfgga.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tjhlwazd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nahepwqr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gekcvaom.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fawauxkh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zoshdonw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3orqijooi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vasvytxk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gsiurpyv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3idsqoxfi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xcoggfcu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uvfkilah.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhiucnxk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kxrjlpnq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3odwlcpwe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3viiygfts.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vxejorji.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xcgmyvts.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbpseykr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ulgcnuyj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cuziomcr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3imdmzmpw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vmvaxuuo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3elcyfjiv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wertiazt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vrnlemki.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3emddqrpb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qryxikqt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rfxbppja.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rdxbahgp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3grwsgxqm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmakzx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cjymmsjp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gxjyynmi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ftdmywrd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3futmjmbz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qpayhugx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvhieez.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3akupuzhi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfftbfgw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xkxuntab.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rgxmahpc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyukuamq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cpiqmmws.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fiecsupp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xfmwgcgl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zmewdhgh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lkgqvndm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbvrpza.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eufgckxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhpnws.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wfhjhghl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vebzmnym.html


<!-- 参考信息 -->