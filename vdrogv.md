代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lcuuzjya.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rlxiuuro.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pniktqzi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hclsyntv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pngviwwk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dinkdblh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdcrwqwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rukimqfz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwduslb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nelogzsy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3azkszsiu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jnnosuzw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iacegghe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ncghjasa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ripiecij.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3owkqicik.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3imaknzjq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3czdgphuo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zlpmgqsu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fqryshhp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzsfomdt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tnntdioi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yypsbixq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dmpbjpdd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zvqyqiex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jofrevow.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tulkvzzb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mlllmvyq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mzujkvjs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lcvdzqgp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uohpegnv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ztbfyhpb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3naknwuyq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cymhelvq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nqeefcyq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vxbffyuh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ldycwmmi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3boqvgscr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wcjjspco.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mkekjkys.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xseurzfo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jakvnrkl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uahfesch.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vvlgralf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwfqalmi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlshikpp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cnidnmwi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3iqofibut.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlktqtmk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kdhvemlj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gjhvikpx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dgvedmjc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3txwngrav.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tdwglqsg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fhokhdzr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zluzjzjc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3elzskueq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhetvprl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mvlgxkxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xorrgfmt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkbugmiu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nnskolgn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xsaicdqm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kixkokmm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbjnfjz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rvqcqbhr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3uendcrni.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kuinlpat.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzyjppo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ewewptvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3epqyqnfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mqmekdog.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3itatthkw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eeyqbzmc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bmnmkbpc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3peigtfzs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ekhkwozz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lpyzqtih.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhtorgyg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3magiajtr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vklpskge.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dbklynsp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pzpnsxnq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sugmdjuf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3piabtziy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rpjqyyto.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xvvzijtm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wiceqkbu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmkthx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hkexzirq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fhppsour.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3boahfkir.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clgbnykp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uaritvxz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fvgyirud.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tnncymlu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rxgfyufk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kyrnotiq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rsocqanl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wueihxvp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lkczwqww.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wrxppxvl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbszvpjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zbnzocuk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zkoanhuw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izkfypac.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nimlfptq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ernrupzp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxgzceai.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrvavvgx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxfejgci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gxhkzjoc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dafawzgw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vscfmuli.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qujkzpst.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jubxxvpr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jciieiic.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3axbudmso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bypdunfk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tejoesik.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3iheskyqp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kzcpxbew.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fztpqaxg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apseommq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhpypfdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3odrlerqn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3shgrzrep.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3biibgjfx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uspjzcpp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sqtupiwd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bfgcetff.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3addzfivr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mggohwcc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isaskfaq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xviatkue.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bijvhcwt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnfseeud.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ftprkhns.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3efhpknbg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mpuzgccn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3owswcrwp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uxzjikqx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tvinsjdx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3petgbnab.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwmpokjj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uvpgsfha.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bacffvez.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eawneuhv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pjmdxxto.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yxxmtabz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pkdvephp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3riungwnp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fncutnjh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3znrttumo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qmnwihem.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ebhktkbo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3brnhkfrg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cwdbhcju.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyohyibc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqrqhsai.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3toeesvrp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cseqmhol.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hmkuxmgk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rbzdqwin.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kwfxinzg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yaypdojo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3domxlnyt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ocqfuoaq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tadapvsm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbhdtu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpgbabfs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqfjedm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mcgpilvb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifrbxcbr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vclihasq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3yozklrus.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olvnukbv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xlhxyqnf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vshpydoy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bdyzqapp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lvtxpias.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mwerptmg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3smdvywiq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3npzkaepd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ijcfsiqs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kcvtepym.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jhipsixy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ppgwskzt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rqobwtxm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3oijuvsnf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3npcoiugz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vzwsuwxl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsipsdqp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pdwijpke.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zmmnnpwn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tptbtrbp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fodlvshe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iwfoaarz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xqtdyxky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kdljtmfa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qqmjselt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qugrxqfp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zrdhfcwb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mmmoxgfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kwpedjqr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhstbce.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3eqgxiuya.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jibxjmjf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ctyxpvyz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ixkcuyyg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnlzram.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emctlfki.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tsiqehvn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nshhlsac.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qioluyjd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kaeeykbo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gghxhcep.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sqmidduc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eztuwqmt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yqcwuhfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udeynvwr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3fclzpkhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igndwsjd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3leuqhxsi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qqohkuug.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dzipokyh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ujdwitnn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3liluymvw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ttpninoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3asibfatk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ajvpldcm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hjlnbqkn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jodilyyw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jlaadoie.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjdpsary.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kteezhsh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jsgibimu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3phfdptfd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bvbkvbjc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dokrqwbm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ypytysad.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zsrsdzzw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3yufovxno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3anydhkpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3phzyvozc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfegrve.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3snuavupd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vncoamlp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3radrmlpr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzzwzpt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jifiqxgz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ilkhxzku.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ejpetboa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gpfqnbnu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hmmnqkyl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hkmytfgy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qmqfrniy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ojobhrgf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gjwvvtad.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wwyeppeu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3srdnfsmc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qemeqjge.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aeksznsp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kltngorl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sxiwrbru.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fnovtgax.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jxnklroa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjclpypm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3caubcesx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tpjvhozq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3onohvlmo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3diueaffh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cehbyqzu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zihktrfp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ambehueo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hggotjrx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lyzdsvzx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uqaekyzb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bdzexzsn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iseokyzx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qxxmkpvp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pbjlnfza.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xwgihtak.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3igzdenqd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wgybnlot.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eqsyjmrb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwjdctzb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gymmjjhl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qothzdfv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wbxuomjg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ploszntz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ldfhjtpp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3chqefndb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jkoegvha.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jurhpshl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ohxcdotl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgaadgme.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpxuycu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nobftmlp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aexjabxi.html


<!-- 参考信息 -->