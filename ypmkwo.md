代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wcigqodr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gkpistoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpywpak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sutrifyh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gicufwsm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vcvidwfb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3trcqokox.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lmcjgzrf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lvkdquoy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3odrdhovl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cvjgdbvo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mlzpdnmk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jgahipjw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3suaesmyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hntuuyeo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3awnuqqzo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xrglpzyn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zflctyjb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gxiwqdmy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vaxatuhl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bzcfylan.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fhaszpwz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kbzdwilk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kvypxwyw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3svbfjmrm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ypphtjnx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tyazfvzd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yyjofhlz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bhlspexa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wqenlhqf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gmazebka.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gcfigqfc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pjvwgnaf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kqmzoijf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqyixjzo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rkrbicgv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hrzznapt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vhhxysjf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nheylswa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fpqytxfr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jkozfcdw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3etpstuvy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ydjuufib.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rpypgcaz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ookcdmgm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yymtoxak.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ezafnmpo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3whukwrtw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3upvxufal.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3veunpixq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ykfvtjmj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3byvnlicw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuajjre.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xwhzmlcm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3egkweslg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3semdlgef.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nsumsuha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cvzhysvq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aexzdkhm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fxtsdith.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cwkmbcbh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bxqfjbrg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdipvrpb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qormmzrw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zaaeagyf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3otmodaee.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vthwqnyf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aviptbok.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rkojkvtn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mgtzunfh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3akryijgu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bictzmav.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3znfnpghi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uctksvzp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fdsvrphu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afyxzzju.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3edfsmkal.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ckzqnjyn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ycvdzrar.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3twgoyfbs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mccwatnx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dxzinfss.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jlaeflsp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kbnnzbtz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gxnhxusw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nseufxhp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ggajxnhn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zhzyjiwb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3visklgcq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxbenrfq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajofjmhh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiaystsk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqlnhxpz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ogquyxod.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tvhagzgc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aurfjwnm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pzprshdi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ohjgundv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3amxxxfnz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wnjrouah.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uixukdqf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3abbjstnf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fupyoalt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uyivsmkr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlsagyri.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ahtrroyh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhkhkhl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3koijnssy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjqzgzs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3asegzpzd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wcihfgcm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nhtgxysp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yjspvwqt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tvgqvevq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xnoqhprz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gmypjtmw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3enealpju.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfadigpk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3txwjptkd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vtvmdovy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiyrqrve.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nhisqvsb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mhyxloem.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3htiwufdw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mgbacnmu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3omptujda.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nrmhovig.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ejgykapd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qfnnbnxi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsbpscid.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ffkboonq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ituxfgmi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nfrfwknc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3diisgapt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ruttvatw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3egetsnqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3puhbwjzq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kfuqnxnn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qfmyhxvg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3liymrivh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qdksfydy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wuboyqva.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyzejnei.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xnfqrxws.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fotcvhcv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3denokghe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3awuunfps.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jssybchb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xyknoxbj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zcfezycd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3unrvhvgs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ckhymsxk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hxlzsnvm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrnwifhi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjurtr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3exkltkrl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjkmgjf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmrbudn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fspgjixd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ehgqorfi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjoibyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wyufegre.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hiyeeqky.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jgkgrnsh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qfrhhnxv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mlvegpej.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wnujphhw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3edvxjiac.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jvvvypqb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qydlrmqg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fixkkivt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgtqbpl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pnarvvsh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cdrojvcy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnydjjgy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xudnndpv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fisnbtee.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ynrxlvho.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ifolxdgh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3twakccwx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwcaixhu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cigfapyz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tkhexnft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3syfvzkwu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vqcmduai.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gkhjylxq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lkzmioep.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lghjqtfi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3semqcmbh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwgkylf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ffysqlgm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqriyuuw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mgxlmqsz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzwjwpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eztdhrro.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wlegsbgc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cdqlcwua.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zmgxxwxo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3daucfchv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ozxvghld.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgcnkye.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3scmhfczy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dbqdrbwg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eorehcdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgwtsyel.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjngylvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjudblfp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ccvzylsj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3btxjkdxm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sdxadmwm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dvqshzuu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jmqhrtnu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3sdgbkccf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qvqqvaxk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bzrjnxme.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vvgwitce.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fxcivvkx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mmtizxpt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3owaricul.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwaawtm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ruuhhkzm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wshjjrdx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srbbgfgu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lngnnbud.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nqqnrofz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wyqpmkti.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zerlpnne.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qwxgudhp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkrkglm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3igsbiouk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3scfwqtlo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wzyqijdp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3apcwozpa.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uupwafnz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3shxzzqkd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3undnixjx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sdtclybt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qfjiavdt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ntarxchq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zfumhubi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yptomqnq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sbtdcsyn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jegjnmym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qeynngra.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wmyjvrdm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3shzwozcz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sgptpqkz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cemdfzzx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yfkufgpg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hwlqwrga.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bllbvnga.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yskialfy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ohlqejjp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xggixelm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3eqvlhflh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3znypbbuw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3heuahpjq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vpklkenc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsttzkh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3crknxaim.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eiiyjpde.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uatlfzat.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ldpklcqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3izdrrgty.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3srbgshqa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ybpxbihc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3utmgizmo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tpgmbkdh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pvxmhtee.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3izqnctqi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zyxsvxaf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3eopmfztl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hpubvroo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mbozfzyv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bjbawgeu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ihposgva.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cjtpzuzp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sqvjyoqg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gyyjmbcr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ecgkscha.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3briflhvx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mthfdhxc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hufecaaj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmczulh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xeccyyoj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3odijodca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvryqvik.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iegdqsad.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hntxlmoc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ziwffyqt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xsovpvqw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pyzdaxbv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3orgoewcw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3edjtirrs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ltcnmymk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ttahubza.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kzzvbhdn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3asoyctzr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gwezdkaz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zxszbhza.html


<!-- 参考信息 -->