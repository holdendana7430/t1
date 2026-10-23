代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rssbqgvw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxnrtsvy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iqqmymor.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wnuhxwdq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mvhfelud.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nltakngu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcwomofa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3griaocdm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pkozyzor.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pdjjwgne.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3avzdccjw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mrmrnwjm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zfcdkqhb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kbwdrmmo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3onfidbeh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3swksyuvg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fsbfxcpd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lfntaikj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccixempu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3firycpzd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zoysjalo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctsjdkyl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3klxvplup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vjlohzmo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fydfsdtb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3henhmmie.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfumwxo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkqasdv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3grgizxls.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cnupppuq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lklcilqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cocuibqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iyaqpqoz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpyiitw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3foorkokx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jjbcqgcu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uxzozeou.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3aehlvphq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zxlmnsio.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vmhhhfbl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3axzfchav.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gjaxbrch.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cqddedrs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jsunsbro.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pzdryqcr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hxcjrowq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tokhaudu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzpzxshn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gvvzjsyj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hxmfazjt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dapbswck.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qivjrkwv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgpbnnv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3juckliks.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rssrdgyf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cspdcrib.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3renssplj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xgxmfurs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rqzmjehf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dwhwlmyp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dbeagvjp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkfoxopy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mxznhawd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsyceacu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nsywbzwm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3eamsxbzc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3brdgmokf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tikhvzrt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3icfazqll.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evxroqaw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jzhezsyw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhxyvly.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3niwwrxas.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fbxykgrz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3htxynwsi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxxyexqa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bnxkbtal.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mtamtnzx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3udyhrehq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pkhgbljq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3avpkmkoq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zwboovtt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vqelrgtl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uzcwccnl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukfkwmqf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kpfpnbem.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3majkpkry.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mxrbbrpf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vejkwqhx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nfiqeshb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rjwomhlx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mfvyoayi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mwfbpeva.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kokpdfuc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ksmvegvm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrshyku.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mozlmeis.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stjdthxh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtvdhris.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ehuyeipg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3whawkyht.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tqbivnha.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3llckzfeg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sorkwpmq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ldmutgxd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zramjryj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nwddwaqz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3iwurtggy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndpcrntf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3paixahyf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kgqpnhrf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhykdedr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3buxhqbuk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3prvzswcy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hgqjrynj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fdsblmub.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jwttugdd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3opecuwph.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cbapmdqk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bollqcuh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wzqvibeo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gpnpgwfo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhjcclc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkqxvndm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3liqyuxlo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3okngcxut.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vltpcarq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zkainabg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vyotmuqp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3shktmscf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hhzavwdz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bwmsuzaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jtroagcu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfettkad.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swobsvva.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ncwjcnmm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfapjaz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgctmffw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ldecphfo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vjauzoyt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhoeksj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kmfqunbj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iudmzybs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xzbefxwo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rryjmabw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xrfoyqbu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3upeqohcr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xdegxycx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qbzkxmyg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qzefyjey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3boajcfue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zasxbxgp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mirnmxbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vrynxxen.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mhpysuxe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3njhvpcwz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3luidkhrg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tonwgqdq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pcygcxwt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ibbwnehl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3iyvxevma.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fihpgket.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3budmyhla.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fyizksde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pvhfakjf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rzomrzqp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tkvcepyh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ftemrvcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3scmsepzr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oawkbljh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kwitapmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3acwzuatd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lgrjngxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjwkwkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ezxpsmzx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fkbcjtbt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nwuofqrt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gygwywzv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ylzwlizn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iavieqef.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rossqznc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rkfpetit.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hnzdqshc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hswrlboy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkzyovtt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mgpajyzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwyhhctb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opokyygc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uxodgivd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkhdmqt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3udepgfjd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcdmjvnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lgyvkxpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvshxard.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tetvqyag.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mgwkxebs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyjrgszm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tdsvsyok.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oagzwerq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hmsklejm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3japiytdo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wfxcxabd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3genlsugn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ntdefvir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3khutkpqm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vjpsyexm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3susxjmmi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ustpvdcx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwfwzub.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3attpdven.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xppmztmq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mfyovzwf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hrgkefce.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3brnlcgsr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bqgsddmm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gtldczmt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yjvykbyh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3cdtglvie.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zjxhgxtm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iwtjsntc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ifhtgywa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kgiujmef.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xwulewtv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3sjkmfqvh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bxawtjry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3drmtdulb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gyhmugqw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sbqbjomj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tatyekwh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vipuyuow.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3holcswuw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hrhqwdqg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3knzjcmgl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3etkoqydj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uhvulyvm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yyxcukez.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tozpydmd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oaezwutb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fyhlhypk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nmznxbaf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rswenesa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cvkqmpcr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sylnapzo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqeqnxne.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xcpanrid.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nmqdmuac.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xbpqafmv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvxcxxe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wghblplh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vyortjsx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zvbdbqyv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vmldtktr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3etympqra.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vwravava.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kediznni.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vyoewgcj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kimaoiyh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jszebcxj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3unpqtucp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bgfyoyqf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdfbfodw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3idpbbtvw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uqyrcved.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ldaemkwm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jwkogmnp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3iquiwgpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dnfzaauq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpydsghk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bwqluhax.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzkzwwb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qjmxsysz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3trftikdt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jftnfsxw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xlaodimw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3utnsgixh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pxyekfdd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3duajcexe.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3thmegicy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wusuwpod.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ashbwwad.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykjivtgm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hsvsisbs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jrernxla.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fzhedqes.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qeobavdd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uooxshlj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dtymuqcb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zeksxwwq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ppkukzio.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dbqnkblf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lkmgxloe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xiiwaxnb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fqmqxing.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lcobvocp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ohctwvqp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vpwbhvmz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3touqgsla.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yenqwhqj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iljrufeh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdeqxbee.html


<!-- 参考信息 -->