代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zaxpgxtw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kqsedwpf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ztrmjtqi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3owfwbkbn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xxpfetco.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3anbffkps.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xcovnolq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qndomqnr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gcyepdsk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydnukqyd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ubzfgass.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jjklwaeb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ziibkztn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jajyczim.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nimkiuew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bvsvabks.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juybfcex.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qlihtvhp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lkthpnbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eaobuone.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vegldcaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3acsrpeiy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3julpxayf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hhvfgvjw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dvdnsbjh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ytifcwbp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hzettoas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vcbhdatp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwzqejip.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zchomahc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsuznrzx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3phepctcr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qzwozqer.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3iazltitb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3meygzxur.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hgsywlvq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3txqemrdn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vckovhmi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3phhmljra.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3azcwvrmz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjisszrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bmvvkxfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3shwpcyki.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ymrpiodd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xmmjzspf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pcodbfrh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xduxkxos.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xbqnyxae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lypapzfa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uknlkkto.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xbbgfgmy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bcjntogn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3plnmupzn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mcnwjpzd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uerrocon.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3byjfgnez.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dsznsrhr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mpvnjufz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bklorqcq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqumxapr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3inkeblqw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3egakeywe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ntcdsnku.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kembzofm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vkodbzlv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sjmagdys.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcrryclc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mkptxuao.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3umpizciz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gzydbygx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3svjcihxy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3aqseistf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qplgcwtt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3molmafan.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ebtvktnd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zbtnsfcs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3owzhnstz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtxgzdn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ghigwpvz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3howaexex.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zuarymdc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3greqxubh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gxfnxtgd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvqqcsv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mozsvxog.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbypmqck.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmeyvhtf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3syiippie.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arftoaao.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fqhfwakb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vjmqdpth.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lvxajuaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3clphflig.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qzldfumf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yeecdeiw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sgdhvvxg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbenzmxk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cqdeyazi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3utgzsisr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukninaaw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iprpoyjl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3piwtdlud.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wovruqrl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hprhfyae.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dxyulmdq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rwskssgx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uvbykaqm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zimdcaol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3djzzqlfj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kkueyjoo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvxewzq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjdhlrxu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gtrvasxo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aawccgsy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yrgbsylo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dahsqxoq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lehnljoo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3budtjebh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gttjdnbf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hwqihpso.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhmoxth.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wruhzrux.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fgiaiqxi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3isudryfp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uqrbfatm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gdyatkqb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oamqaxrq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ixyocmiw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvxwzyr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qxdrdsqb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwckvvzv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rmyfdcwv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hzlnjndz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dzgkmizy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sqepdxit.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jzbtcrcx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qrzijhev.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lbzgqmza.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjkhdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yjczjogl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3razhgles.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rufohwdd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dpkyqrsd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fgsyooeq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zfqtmxgx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tysqrtnh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3olcpqgmt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfbkmvrv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dbexjlap.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixglgfle.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3soqhdape.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mfgqpntb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hamyzngc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nqvmsjxg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ydrfhcis.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ohhgznil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jayjfmng.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mjgfrert.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xsgjrfre.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnyxfgl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3paajofcg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvsaajw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kizgwzvg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qegavohn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wwkhgxyt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wudtinco.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ybvvpuvx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hoomiqyh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bkqmvspy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mwzzkdqe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tmjuuobj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ygierzxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gowqalnj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xovfmujr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgjouibh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zeiarwiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qiaiyqhz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fjomsirz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twqjifwy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nadvzogs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kguxjzoo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3umcrzxff.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vsmtadgi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ndglvmbu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwpbljfv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oblbdaon.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ebczoxuh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3trrlpxdl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gpfgouqj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ssgsbvpf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vvnghriu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wddheftq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lfgfhnhz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tzcwzbth.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xixgytal.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zfbgwusl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwcvzvh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bnjfoqlm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eubybvkp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pqfxxijs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nnifyyqd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ligsyykx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3myyaznns.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sraqfspe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jiroqsig.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aywibfzq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ersmshax.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ffbchqlj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3oroiwrgf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cuyviewz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nphqpvlx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vdrufgci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nkjvuxss.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vjnrrbsx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uktmlica.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ypijmlnr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rhpjmzcq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xxmvxhon.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jpfvbwld.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzwgmenu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oocenace.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cwjblqke.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vumaiwzg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fusebxsi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wubddgxt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pgzgauox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3apigfltt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mklqtfiy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eqafiajr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ibicfoug.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ylfvkkgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3okpsmriy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dmjfajli.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vuzwtdud.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bvlcnebr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txazikif.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3grybzyhs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hilspwhv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gbjpwlcz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vahygkct.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uifdykzb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ikfrefei.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bbuhjafv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fdxtsmnd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ahhedvjh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvfprsuh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3czbwtves.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xwmqaznq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zuuqmouw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3imycskvf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3airuklgt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zyvykzzt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fwaivvcy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3luphqiyk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vanxnrjd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pjrxektm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zprlemch.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xlwbodrb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xwzolvga.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fornteuw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aukrvlxg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaetpim.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pddooois.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kuljewts.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qhprtpjm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfyviwop.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3odgjqnhb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vraikfpk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qhpmlsmy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zlztallg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tjwwjduv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qmhdpwgp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qggdtjjp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xcujhnfs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cgymhsaa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kueioddj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gqtkpasc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dpjunvbp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vazxsuju.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hfemaecu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhceljc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yqltlcuq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3iaqimvvq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rsdhnqfr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tlowaldm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbgqzoi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3scscixmx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3frmqmckx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3suyelckn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vxzzafyk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3verbudtc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gpezorrj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3delkkxav.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zukqnrvt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqngrwzy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hadnuidc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zcgypfnm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3exgbfbci.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lifshvte.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3heggxitk.html


<!-- 参考信息 -->