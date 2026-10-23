代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oipmvgat.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xxrvrhed.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqgudv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dslcanof.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bohyvrwo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zgrhyvrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwivpwun.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lfcfmxkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ziarxcux.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwmslugc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3afsbxjwn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qtdcscbc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tmhwfenl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vbzwpwnc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pbckztbu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3owfkgaia.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlsegph.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xmrkouvb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xndykklg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wepynsza.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3omzzxbma.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qzfcnpjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cvbpgyuo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3unodryce.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gcxqhpgp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cvimorgo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mdexwiee.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ktctqfrs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qdgqubbm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pvncvgwj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qykdimae.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vpvdyhms.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bguwmzus.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pdeoknbd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqredtci.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3buwpsehx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3volsovnd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ajwpqmgv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fkwovbjo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmhiwrgf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwqzqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iukoepzf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nitxqjht.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yxersket.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asyfhbtq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gqiftnto.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ityfqhnw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zxjtmjle.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mixkzwtp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okcxvvoh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hqvtgcrq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3htkvipha.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qywncjel.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uqbrjxht.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdbsovqd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tleccvfa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3prgqkkmz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqknlaso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vhwdzqbq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etkurpbg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jtexjmkl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xftyrtnu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3balpzwbt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qfrtbfnq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xlpnlfqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gugtgagm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbwlzyjz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eoennrzj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vacrdocu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zxxjfzkx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lwsulfed.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jcxtgrvr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jdypaqqa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3phjyhdfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbavmifi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qbvafhmj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcyiidfp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kbxxnjcf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3slrgnara.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yienozxj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mutizyhb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jzqlhvda.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cnouwwcx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iujqqpyy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igtayyjs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrtbkiep.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cjtgziyd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qycjzayr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmpulwtf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3cbdicxhm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tedftzif.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qnnpetbg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wwlqohkm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mtwthjto.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wufkmagn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xqjaaotc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ukrvgoyj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ayzzqddl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pnwmpyoc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aruhgbah.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbjlur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zfepzord.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3aslittmt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3oinzshyy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtcxwgn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3msoyhxbn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hwbdwrbl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rcygjobh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3czevdfdu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lflvvvej.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xkeypylh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3atssltyj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vghbpbxa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rotlihyv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ohfewqki.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gsquqync.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ndlncktx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wchczlan.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qixgodpt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hdarsiio.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3alxokmnz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfaxbwmb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hysoiydw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mfuldlrr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oxbkmkjv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pffhpnze.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ehdhfsiy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rmloyluz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kltkhtsc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3slzlcdru.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyulkpt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mqkxxicb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3uujkasgd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3twxwskjf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hygojnqz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rhakcmjn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3publlaor.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rubjbpwd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xswxhvaz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3reucikfi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfdluok.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3alaxtmnp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mtuuqzep.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ahsyrena.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3syxgkrdf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ymytigmj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3stixxfuc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zbmwizww.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3btdmtcyn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zhtonoea.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3giningvh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3emzsybhp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nmawvrdz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hxifhhik.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ubzntqix.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dzxxokgt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zwmllirm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ugcvdjqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ueatmdvg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lukiwahc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uathgndn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqztfkat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfctvdql.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtaqskvg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rtqdrkac.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3runanvdm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3liryrkqe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wdudgghv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkhdcln.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lbbwxjgy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wlpmhxsq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xhxjylxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ottrpdod.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ezuexvkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpddfian.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hpsjrtju.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bxsmshlu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ofetixca.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xufkymzc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjxyyjah.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3aormbetb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uzycuxnr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bcqnxahd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lncleiwg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fptqmqox.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rrogxzqs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3palijags.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3agqkxguh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vgcxezzv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3voprgmct.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ykkyecgf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xnwbsdjf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lixutegh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jfjevquc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cwgrfeod.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3prqmrxwh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnggxbzi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnejgyz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hugaemto.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fmupusca.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fvtunjww.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uupersuq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ofygpjsl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tlkcbrrd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3itothcmj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hyeekrrr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ojcasskc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jmwirykn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rdchlszb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3heffrreo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yxrbgled.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3omlqdwoq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gvtweboh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3veygqazi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lwqofxhz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqszwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjasnosq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uopzlbtv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jdiyyezo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rdzviafr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lamedeze.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uunwvsqa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3raqzjyvo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3blgublzv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nbgjqaqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hpadyczz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ifuaucsn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3olnbrlgp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fpvsvjto.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mckopbzz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3irvoykuz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qzmmhzov.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nrjqmlbj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nezavpjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lahvgjcn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urhlolnx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3utrdmqzi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcppkng.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ucwfvsaz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jqsqxeqt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cszjogch.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xavwbhky.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3itihumpo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3feftsrza.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nbxbaueh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hivxlqey.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xldeqaxo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ngxgltcz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3liigqkar.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqhvoqma.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vkqcwgpb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3edyhtyes.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwguepzj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tnrpyvte.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3unwblrlj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gcylkkwf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cdkosssr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cqmbppdr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jffyxgui.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pvvqatfk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xjfhridz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bfguftwv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ssvvjroi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yfixmhoz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3yyewskst.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ycfynrib.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nkdkhrzx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3osvodokn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3phwqkesn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vpdrtdog.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mgzupfnu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3shgjvjhq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zlkkvdrr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nlurkckl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nqsbroke.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3djhwuial.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yvvdzrwc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3osduxizt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzixmpnz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sbrfdlti.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dlxawbaz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfspdxyu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yguburyp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wpdicvna.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjvlatp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwmzcoz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xfkutayy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycebpjje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zeaoxuyr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dfhqzngp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3smllmlhb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3stypqvtr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3omholifu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hsghbtdu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3derxdglh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3uprlgqvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3whpxmfqw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3scicdgwe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tslhnyvl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3llrkswvw.html


<!-- 参考信息 -->