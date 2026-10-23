代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3seaofdqi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3grkwmlfy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3elztsqgv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zcqzysmv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3doptkwht.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3auqoteui.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3apqdpxak.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wwjbkosr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ousnpyvc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3suejkmyc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3erctnyze.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rgphgept.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvtsgcqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xpabjurc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xmegsjbc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3extgwuur.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3disbulfe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3idwslwcy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3erpwnthc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zjthljjd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dtkxmkdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ngkkgfex.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgdcjrf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cneunavh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dwoscttx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpgleq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jplwaqhh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vbnqsgkc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ktaavfjc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjwsnqv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bxmclczj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ggooural.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cojmqhzt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xctqrghx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uetueeeb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wstgbkxb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3diuxchfx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqppao.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hccylwkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mxfrtqmp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hjvhmlod.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsxukrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cqdpgtme.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xphlpsdm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpebmop.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uglnxape.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zbxgulww.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3saotnguc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fofnqxfb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ylrlkpwm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3quktdsuv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gtybuqne.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ccbbipnd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mmmvevxy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mnoksylt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dedmcqxo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xelesyeb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dkqpbztm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qotpjdgi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihlbpvwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3grsfbheo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3arxyzexd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbvfwnst.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wtdbynoa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3smdcvurn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zkbeuavy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3luemfdxy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aezemfzn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dcgqdakr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3itfftdwi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iocohgti.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qpqoefjv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jkaphnwg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ezqbjaxl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3agtwajpa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzcvjamr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ipzclntv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbtygyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rgalhnee.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nwcyvkqt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qvxxbztq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wkgvbuot.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hqmvpdrm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjcqvgpe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3droygsnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpcwwcp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnqfdanx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ddvlyarq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohvnmjmj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3takitobh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ujcwbrgh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wxdeytkv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rkgjwpyk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3aqctdwlg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vwqmzbqp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bnqqgnag.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3weqlrwzb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rrypijxs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xfptmtqh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xrzsueph.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xotfnxvm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjzcbpk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mhizrfmk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vosoitkv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3psfvdpky.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rewrxoor.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3scacharb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qdnizyvm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lmubxszf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3caehllzh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyrhlhbv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbyizps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rvomfppm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3isdeluqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tcbwkkyn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vopfvqdc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jdedvqyd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oqoxytjb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdxcyfnw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qmvjskge.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fnzpqfzg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulbdhqjo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fmdyluhh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aplvucrd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wcuyksws.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3squegccm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftljllcw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ljnvhtfj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvbgool.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3sougqqid.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3thlsskcf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hozcpblg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sufksofb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ycabhmvy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zzlmjifr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fhnyfqjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cxxzvvmr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kczsprdc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3riaurfkv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vodssdlg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ffxxfmvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wnszkrtk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vuxrfbzz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vvzmalae.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjuaqqu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ucwnocjy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hqkgthmb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xpsjqlyr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwvzkcpq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvmcksak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3omjyuooy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qtnmqsnn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zpfxantl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ulhypsqe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3whtfstcd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xybvmgrv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3soqybpvh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unpiqzap.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wasispmw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vszrzhcj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zinzydkv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dexlwwta.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dscqanaj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zfxmnfbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gixkoddx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxednwb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3plylxwak.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oigbbhos.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kkqnkugk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jxrnqjrd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rgljqjux.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3brhihzdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sotwvetv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tpelsurr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpzxeqxl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wycjjcci.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cvyjyqrh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxijeiva.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxikbi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rxddkrxo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3pamhezpj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pekovpni.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zqyzqsby.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lexhgqtj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjzeplis.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ecbstyhr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rqrzqtoo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqazymko.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mibziqbg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vchjsads.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yhtdbtlf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qskpicby.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jrviwokf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hxhismni.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ucxcwhim.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wjxwkaxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhpstbc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wjegsfwk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvslapvi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bqlcdevl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ccqfzghm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3petidsdj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fchhuacs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dqdodyoj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tnhbkgco.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3asodjqmx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qgyjqkrq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jfxhnqlc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3navwsjqc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rwvblbzl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lghhtbzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3elrwaysp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pxwesvmv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uuzwlsgn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqwczkp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3icjgxaid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gzvjkafu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3acuzhqlz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dbnndauw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bdqepozv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3limfyfxh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbpxqwg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzaitbzd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3adwanxbf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bsgiyxsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsfkxqe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jdkzceyn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltzviwmu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qjucsmax.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wkyovdda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yclnuweu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3codpeyhn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lgnxiuzk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nrbjgbqf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3orbgefjy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hchqflmw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vdnnrzwz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3evlkxsgg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3chkualga.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ebpfgluq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3citqnydr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bijmztrf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yysfkjdz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwgtcbc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvhbjwi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jxlxwhkx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rbopzxck.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qfomqvea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fsedxdce.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jokkobct.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mkoniuym.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbcsyoy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eywqbjwj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dnpeyjox.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3diylxsyb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kzoebjrq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sqneqrvh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eeidywii.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qdpknmhu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rgguxlzo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3huwtaesd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lwjfqxbz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qyxywovk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rzsovbje.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mbotywxz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cqynrgsl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dzpbejab.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3owrtfedm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rlazlmim.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wpnqwuec.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dqalehsk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ymoufwsx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gylvaqob.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3aevqneov.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wejqpnik.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpjuszx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3upwbyfxo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbplnilr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dpxqimmk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wexnnfts.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzsqybcu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3usahqqpi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vtnzbumz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fwkbkctc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sokpotaq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mpgzdezv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zekvbafi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfcbycoa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjpympuw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ctywteyw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3frdbkipw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mheaiqxw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3uhfrdsdp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ielielhz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cgpmgwfs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gxcbugir.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orheozfi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3esepwqwm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pajvaxxc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dopjedec.html


<!-- 参考信息 -->