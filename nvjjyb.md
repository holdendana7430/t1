代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yiieddqz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbjjyhy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uwcdqsfo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bcdzipxs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uzncwesi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jwkqadrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3podyadma.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xwjaqoui.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kuryzzxl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nhjdlstk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lxpyscam.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nmrzpfvg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pibatuoh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wksyoyle.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wavecwfi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cebvdids.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gdwctcmq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxdxrqek.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dqfbrrcd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3koybrmli.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fqcwfmzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tiphbmzd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ryvoybvp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwesuhe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pzbxwucq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hropatuh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3plemxiui.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3enatdtem.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfkzcrq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3llvgilwf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3utnormdq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aquauphc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3netjotli.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhyudlkg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dpkszpet.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rmzgnrhg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ypyqjkft.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ledqrhgr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbcqtfw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aybkypdk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zqsuaijt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ixnjhisz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hxhlbcjo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fcxqherk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qrugfmwd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3djaqgnak.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ohktejhd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3arsskjmg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rvklwcrc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3drkikify.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fiahjfuz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbrdzhg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fhvaeoed.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sdqxcgtl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3boasaeqi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gdvkblaj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tewcspqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kjhfkpnr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ydouuflg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ucetjywm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fpebuyar.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wllvbazg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ucjhcmbi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dsictkbb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zerzwxum.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xcapsult.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sucqjmjo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bbqiispo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jksbrzsg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3svwikbsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkalozo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bsyephsh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3auyksbgk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3akgatnds.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amxaatpk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3exnstusn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wbvhzoot.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qeoitavy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unmajasx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hjwnqhia.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wqvrsvjg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qfoksuoi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xgitmjxg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xksqxkta.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3taprclyk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3anxywagg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nbgqinds.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uyrvpibo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyaxhnhy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fgcwcwbe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nrcjfofc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3axxedmcz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxonntog.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qqprxpzi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ndudmnki.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qfopfyvg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sbrkiigw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wydhwjyc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbpngayg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hvdaovde.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iklmeiyu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjmemhbe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzzafosh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qghvtcsu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3afcjyjlw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oadclprl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iytpyibr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3veyudgmw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qmcauodq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xfdfgpbs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cwsfnavu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3brdpvvzn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wunwuqwy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bplhfxcl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ooedigye.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3joandcld.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjlqtnta.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kzrsjoiq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwjgpclx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xoznffku.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sjyfcxhi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wuwmcbsz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vtezpziy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bgqgfmzb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eygstbfc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mrgsqock.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3acabicvb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3slywqhax.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3acovnqjg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipppmeva.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pmjldjuc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dtkotxlb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwatxmgn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kpxfmigx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3idypntwg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwoksyqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vnzghpeq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rzfdaaba.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zxcfqoge.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ppuvdpfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3obhsroky.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cbbwgbmz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ucpekhlz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rdkafnky.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uwgbiqhn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rkagqbjb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xxmchlnn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qhumdmgu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnuxojl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mcwipoct.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bmkvkeaj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3amfehmfi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ffwjqupf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3faalyqxl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdejawvc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gemacvpf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hzdnighl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ibarkvnp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fqfpwbvq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cmjkhxdn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wurjhmrz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vyloeolf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ggixjjrs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mresykaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3noisomvv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xdsvojcx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqazshcp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whmaohdb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ronapjpv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3miqtbvxx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ukvwoyat.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kvcqtnbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkqucxuj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dxyindla.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxinaol.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3inwvxrdh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ywemzgjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mgmodzyu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ixgqpcnu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbcjeqi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tgndnctm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjawdyeh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qtxjdefa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3glyokcuy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lkspzxto.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iuacrnty.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zdswdsbr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lfwegcrx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yzbrzpkc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xlhpotye.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ynxwundj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oqocfixy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ffyzpcqz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3icbiqymq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qdscqlia.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fheurjvi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mlfbhgua.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hqzhnuop.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yzqpwbth.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dirzzqxs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tjzvfytv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xaqumyzx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qcooiccs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzvzkgro.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rirgpupe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfjfbca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcalftdy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pdbcfqmo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3quzzcrqd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhrejild.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gvvyovgn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3oihctptd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ktjhedtg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qevuyolj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vjjvgyqm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uzawolyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnggumky.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zmmhbext.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxbeduqs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ygdlzcvb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cnpkjrpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3raxxbvym.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ydstbgtu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3smydiepj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hhnolqxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yqeswucl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3scinjuhe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pvpwheog.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oielesju.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kxeaacoo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgqinsjs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3btamutuh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nxanwjlw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gonnrbna.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3euegpiuc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xftfdfeh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wqudxghv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wmihjqcb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hbdquykl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bvurkudv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ylzifbhh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ftsrkwsb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ukfwlkay.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xiuyovwj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3plmgnhta.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kstqvnat.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3osqrakqu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zdbfrtxp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ombvesqe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kfupzesl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhsyzcp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3korygaon.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zixpxrmi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ofqnzcen.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qipqerbw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lhllerlm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rlqwgaba.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3enbxwyiz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rtbwgbav.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3udxymjyx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zcyasgal.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nshattbz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bcejprcy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjiuznei.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bcuuopsb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yifhvlbj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rapunsoj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqoneahv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ruchrcbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rqjhzals.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eftvhbgb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eutdfxgm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zkjpcbqe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gcoteklr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3indsnuve.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmpxjvx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yopolsjc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wknzodpk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iytgvsgr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knulomhe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xvqqdmbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zydmmbgw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dhgenlsg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3oplmqpoe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qhxkxoxz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3izwwmsyo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vobofugq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3afudmrvx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lrzdexoh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kdmbvpbm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3clepdtys.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jkhyqgqb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zmxlnlft.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3pvbjxwiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjuzgxmw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wycoldfx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ktnyedcr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpojuuov.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wiwomnlg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lpouarzt.html


<!-- 参考信息 -->