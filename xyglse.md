代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iwdulaun.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3teaeypbm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lqntjlcq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rcgsnlxy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vjinjgys.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fopdiwbl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhqkngk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mwesbppm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rootjowi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ihpbkrcq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzwexktk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cylzacpn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3laqdownv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cggojqgh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3krpmgknj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jkbxdarh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tocdxjdw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lngegvog.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrhopkx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xxqaykbo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtxunwyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yrldlmbs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ugxqyayl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mdjwtdpa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gbooryyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ryarjnen.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pxrygjkz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3njddpcpp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jekmlbpq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3befdibiy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ubvpiacx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sshrzima.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3orwgjteg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xmwbdkpx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwyizkjs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qppdvggu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3baxkkmvk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ekwsdnfg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgsnhyzv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jwvdjyly.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zwvibkij.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wspnugvq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qohrpjlt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzxsjoqd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxmwqrn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pcyxdxgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xdcybjkv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfkaubu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plzwasnp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3audksqxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dvylgvoy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jdxlnthi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mnamxvgy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqiqjwd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3budurbrc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hzxfxyqb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jivstagy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kldntjcx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3syzgjtvu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vqarsyqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3epbkabcd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jyzmiikz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxshgxg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjafoya.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rffudtov.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qhlwgfkj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3imsjxsbc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mtgghfph.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ypplemsc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3voxmeodl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qotonlvs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vovfghgx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xvgepmke.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3auwrdtfv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fmudwxtf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vdwpyfao.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipaonotd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3woxjygor.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3opucunvd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrikqbug.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmtgwhn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rdcnoenz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gmosywwk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mipfapge.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fcvplxao.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yvawbtug.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bztnrcnt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uonfzite.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqhlgo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrnijtsq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynjulzzc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sbcdqgrf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dabckusp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cmaygacn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nauivure.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3syijchtd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jeoocbma.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3otnvjwya.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tainaohz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ecanmwki.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uavylcro.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bfqyzobf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hkaxolsh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gdrjiqcw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jdfhrxto.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvrftiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3enehfdxo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pqywblec.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lwapupuf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ntimhlke.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fwgsdjry.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tqeofbwd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vjlpoirx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zkdjyzhk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3klwhjszs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzvkxbzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hxlakdlz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fitxmbbz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tlcniflh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3oavcurym.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hcjqtwcq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jmezjzhe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hntypgys.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fyritxzc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3afvzrsmp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gaocnaiq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3edgpjclb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uioeqlyl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amxsxffu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gopkctdk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lekbbkeo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xpopfhxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqjeviqt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ncurnmrr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpkzmxqa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vzcrdyhi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qybftfqx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rgcmwsjk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xfxkgkkq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nljjdjai.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jmybelnd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sremkgez.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vfcvngfk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arqrrhgq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubcfdhpo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sntwzsks.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wthiyljp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rxmckpmx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqyhkhq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wvvgjtif.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uhyezanl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3brsfegfd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3flnusmnk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3koqhhrac.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3trgexvtg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xqchwukv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qurhozro.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vjszwmtm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hvopfjau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3geajmfvj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3geyrjkeu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gjzthhjf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ikkgwyvj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xgutkpdh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jwlntbcs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wonfawdv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kwkizapg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3spqkxegw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wkwaahkl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ollnniyh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cvykmvta.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbpwmfxe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhdgiit.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ytuivjwl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3afwocsho.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ujpijhfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upwmmjzf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pygnlkxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxlstd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hwtbppip.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3twizuoxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gblfydua.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tzmrplxi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hynnfdim.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qzakydnr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bnjkiqgi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3welqsebj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kalokjcu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smmwaapp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nmdjdoye.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3towpiapb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijopzhyn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qduigbzh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ahoexpos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sazkigfw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3egmushtp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kfttgexn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3npdglrct.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jiktbcuv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npbcltwi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kembynxc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nypqvfwr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnptytc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fuofywlx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3glpcpfbk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3htqimsoj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3skfbyblo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vexirjpi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxwezb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vsffxzrm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dsuwbfbj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ejbiijlm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rmvcjisc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sxnzfgww.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wlyofrvb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3voxaavmr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zproutoa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rkqygyns.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3afwnhjzi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cltbwfex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uhhtshph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qhpgbfhj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3phlunikn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zjqhrbdz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3osuhjytp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eozivhng.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfbznwzc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pawhypzp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cnvbydif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spjyoaks.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxxjrvq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkbcfggh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eiogromw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cpudfffj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fdrphsle.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vohxiaqo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bwhmhmel.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3delwwsgj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rxhptorz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsulptor.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wfiktkhe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3iaepybcz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gaevymjz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3swdbosak.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fnrhbesk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sokaazve.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3trdspcok.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3aoqgodjm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qdxlawmm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3clxaolma.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfurgpm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jzdkfvmc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eqwsebgc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhimqtif.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fdhcuisr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ibprksdp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sismtjvf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3eqkdfara.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxyrliea.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jwbjzhgc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3agpzlevb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjcpwewc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wauobvrv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rwyypkou.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pmjkmpzd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vdwtznny.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bkpckxzc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3amyjsoue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3icafwsnq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hzunyseh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rraowyhu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sdbiawei.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wbenfsfb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yruxdssi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zjxorvvf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cqnxzcar.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jmbjygxc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3accknpju.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ccouuhfo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqmznjwq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nlwfhujo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ppwtcqhc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pouwjwgm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ixeyturt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dzsislhp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sqouuuan.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3viclscyt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jyywnimh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fezxwuvn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lrepncmf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvgmqsbm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jpyfuhwb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aubyikrl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gaslmuzz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lqelutnb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtouscld.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cbxjmnfs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xrvekfxw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rktejeft.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxvikxs.html


<!-- 参考信息 -->