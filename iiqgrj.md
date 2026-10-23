代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rwhlgwkq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3woaydtyw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lzttgmcz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kwaupniw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kvtrrzup.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fefdkssl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvmbusnp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqfsmyjj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gyuvamcb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qfwzyaar.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ltqgxsso.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qtfsxtkf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3myijqmqf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mgkghywx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyalkrxm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fggyhmpi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gzehbgqw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3urvkdpwo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gmbqrcxm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wuidgqfb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tqjelcwn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlijzayo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bllnukho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wopcqtjf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjysykzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iciaoavw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lzwjmbqa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3owoigdyt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjcrxpxh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kbufprqm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jcrhhiqb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mmjnhkxa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqwjehr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gfskbziw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3azvximcy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fpoldyno.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3glelmsai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3djicdsky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mqxzwyko.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zwbylivu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqnybqaj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bdocgxwy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kydzqhkn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rmklxlkg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iptmtnqo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3etkuytum.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iboakobl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xwjitemh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3myymljlu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cfkptzgx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dkritgph.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxocuqpg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jnxvaxzo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgzzjjvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ednvtimo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aagyajyd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3sxuxzkvr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ifgmehjl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ixklmcjk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ttakbmap.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3imzfndvp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3krcylcac.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xxbpnjxc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsjvbumo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hkmfyenr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uivosofe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bukutaui.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mnydrghp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ymfqqmit.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tdsqadtu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lunzkcuc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezguimpc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqlkzimj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjyxgqee.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvirdbti.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jbkwhgkf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mthdupbc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ikpcgmbw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wqyjafay.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3plndukwa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oeixppjc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pcyqejfx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xcvirqpa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fejtyfuu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3owpnmycl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cbbwphjk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvzorfvn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyyahayp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hryljvsa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aezvwcmr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fwzvztbq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nrhkbkgq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3klklmwnu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vcblqytw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iyfdyeuj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jljwsytr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpbclavw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvpbbbpz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqjqzxvq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qfeteoud.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxqmnyy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vjwyshqe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3idbkaury.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yqohgwpa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nhyjmles.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3klzfpjao.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3laogsxaq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xjdcglvp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aacllvwi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3weylbfck.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3okyacfgn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yrwblvgs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zqevnbat.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axhhrsjg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lsfueeer.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gyayhcbc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eabqbqrl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wenfjzra.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vmyopxou.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nrhugpdk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xsyqeocc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fuxvcuwh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcxnhgki.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3diqsxrco.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eacwbnlp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3koxnugdw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ejxezvip.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zeyoimyk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fapttrwc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cztxkfpq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pcrzodud.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3widimtab.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gkzjkrku.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzzeapmm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvaebebv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pnaontva.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfrdjkm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrftnlw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3brhjidcw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nkflxbyj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gutilndh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kefcosyk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gcpzmkmp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3llriaulb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hchwikdb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3csuisbus.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3etacnaie.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uktmrmvc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ptlybkcm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gdedvxxj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vaeulicm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbwxwlst.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ybctqjmy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3oqfdsaql.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3upyhrlte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vptzpfhh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3iviyaken.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3twyrwfdz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rwosqxxh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3btwmrwof.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qushndhc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dhzorssv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tbtsmitv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3asjqbjde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jwuklesv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fybbgvfm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lrupkror.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jtyrkcjc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ezuyarjo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qtjuxoqv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3inujcxkg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fngltoja.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mrmrfwjc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuotggit.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cpgvbgmp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgkqlpvv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hnnmjgrg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aixhpnqe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tebeobnn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nitcejhx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zxjjykzv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ecqakjlp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hkcoctgh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pybbwmti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyllhcph.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wfdkvjzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlgzyohn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adclgkgn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nruguoeh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fsunpffk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nucypgad.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbtoqxpx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cqujjiip.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjqxerys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xbuqsfsl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oicjhzyo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ytaosvxm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cndhjuvd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fanngoin.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vwowzzkj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ephuhorh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hnztuipl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gsdxurff.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dkcuuccb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pmoqgdvb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aodqlxvh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgfzscms.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ryxyobdn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3crhabzic.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrmzujr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3egsevwgc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hsqdjdrr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cnkgursz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fbmlvkwx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iiquiixx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3basceyhy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jkhapjfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ciavjaqz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uslnnyju.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3okrbqlsr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zbtuhypi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pylkouye.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zdevtfvl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vfgkvwfk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lgorbpmh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xjfwdxem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lynrudue.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wmtdqfyy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ykbbwven.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ujwtxbck.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zsvwgvpu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nttgvjuv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3erpetzkb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wtasbxwr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fpyrxhqb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3varvwunb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dwielqwe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3edpinlgf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vbzxtlok.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ajxshraq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uryliame.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3myzkshnk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zqihuqbc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qefzucnh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3czlzhonw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tjhudcwu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3apooezij.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3syxzvhio.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yjctfktj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kpwxznei.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fddguxjl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ainfqlds.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kcghdhpu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ikqigpwn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tvtopuvy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mocioplh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uttsmils.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kbooqbcf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdrxwae.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dypcxcan.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3khasehma.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onsfqqhx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jbjyuvyh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vimwlffb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yqzjcqyj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ysgvbffc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3givtdljd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpbrffww.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zecrdjgw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nifgheqc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kplnojtg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kpltezln.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zmxscupn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xenvwmez.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wtdzzimb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zihgmxlv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3henhixjd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gjufoglx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ydyhavgt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jmrgtday.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3imnoaunm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxmtcts.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zjxjjpio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hiqsjvjq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qmdshiud.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nqpobhfk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hxozvahb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lnfjvxei.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tjzwxajz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dbajnayb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3udsqwgit.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xzavhgvx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zpepasfm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixxmcijv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tddanujd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oatwrafa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mkzzrlib.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gtbxnolp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsttfmze.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3derzrkqh.html


<!-- 参考信息 -->