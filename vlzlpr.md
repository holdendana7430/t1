代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ngaivdyt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfknznpg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ujhsgamr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwevbzy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uuwdugrv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kmryvqsq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kurcmlbc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mzqixbrr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mampnhik.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cfdkqkoi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbixjuj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uizbndol.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ctczujmr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ttajjrup.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ixsaqagi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zsoarfgi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eprhxnvh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ygmazubk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bpruvxwz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dyzwgwwe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3naryxvsi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ohotdttu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qkcasdcz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3poyychhl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnuqkezl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uedzkbej.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3klpwqwza.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3myitsitf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3aenjoofr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3conuwdae.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3srhmrkmh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bgbiowpl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bbnacown.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mriqmtiy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3omgayibv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohvwgxgv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rvbygcwh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lmtlzlro.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nvsbdgzr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3twtysyru.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vwgkhzzu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wolqwumy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nlrvftvx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sipilalz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qzphaxtu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3njrxveip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3potcatua.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3idjhtcrv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bibevepy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yaiprias.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iktxhnus.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uujhqzqw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzovpcyw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3urpoaoqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3axauxxvb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3awyfjzlm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kyeygnak.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oftsbbvn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zjthbtse.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3zeyiwmvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bfmeuiiu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jinkohnf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jrfvbjou.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pstsyuqo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3noupjehi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zjkjlcyv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wmwaknmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bdftmnvu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hbkgljxy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vfmzdlla.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3knzissru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vbywparb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wqgiljjx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ouipkdiw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yacscohu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vykdqmfw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ifbjvahv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lzayzili.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fqhsgzxh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aprwyoir.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ynylribg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3inmjllwj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kpnmeswx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fehajyfh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ecwijvtk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wlqheaps.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sixfclbb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eqmopeda.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3osajbuax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxsehcm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkxbduc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kcvhldjp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pcmyuddd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wswzjnpz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dxxolbph.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tpovggtp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fqtxgpel.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cyajzblr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wnbtotyy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iyfjcsmm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ytlfoomx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vijahsai.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lujopmxk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kbadipev.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jzrjihsk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kgwfrdiq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdbibehv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uwvukjye.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hdzljwha.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3snyzdydx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3luuvtowt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ytpcwhkq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3liuoibqm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gmmtzlez.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnkigdel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxkzigjk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3byhgcmbw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ycvqmesy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xcsikrjx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3duhwmffd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3desqifil.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mbxzuczs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eopwiwce.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nczkfzgs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahwyadke.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gwaywwft.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oywltzya.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cgslodph.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3awshilww.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qwrcvrfz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3syzkwfhr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vxvbhhpa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3njjqhkii.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3axfcakvb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgwukts.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gfnkscvz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3itcrusld.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mzzoafzm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rnmfiijx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rmzodcfw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zobjiyck.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ozdlhcnj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dhfdsajg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nefsariv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3umkiamen.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hspwuzef.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xktxbebx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ezediqqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qrnyusbt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3swfactwu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esraajgo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpvciega.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3thkkmjij.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mrnzlcfl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eswzpsiy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jlppwxyp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3agdvcvhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pvxcqpyy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vcoqekzy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kdigytuv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3peahfkjl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srjlwpse.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bguqrptw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vijndumz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmlxfeae.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbixhdz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tqclljiq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zigbhmaa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdxwfgz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3drmojpms.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txrcbgqa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xptrfden.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wlajyxco.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzodpvig.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3haysdibi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mkacbmiq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ofupwrgi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmnxhykn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yrcfvvdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nplorilt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xfpytgbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3joqrhked.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibqndauv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3smbwnpvv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3laxzzxnw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wibheclt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jmbjgedo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qvjlhpqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzwledj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3icpuxpgw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yohpcwmw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yusanrzm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3utfqthbb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uwkheafw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3alotdtan.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ttbqbrhm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3otelchoq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzftmk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fgmepqov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vukqhzgf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3puivdoov.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3atoxaqoi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ujgccpui.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bizdlnon.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3axidseoz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqqmtvej.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nxqxevtt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mzqfrkrj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mxtumvkk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dtceltfa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3smwsnrrm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yteqvkaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asomxwzq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wbdyvpds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emdmkcsu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ragnbfho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3aczaogzg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrcrqve.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3edfnuvbr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fsmjjggo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzceilwh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dufdjujq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ahdcygzd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hfcyrrog.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fcquvxjk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iuzreltn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wnaocbus.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eulrtiqv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hikqljrm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lkdqnpuj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pjmhfzkw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yjmrvdly.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pjcszvea.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3haygqyco.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cbpdulte.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yxlvzned.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aftxhdls.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mynzcefs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3diosjeop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dlfzdcck.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3eyvebpsa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwuqsfed.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3caabcqit.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mdwkihre.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pnfywqob.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fbscyubm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wlvpoyjf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ksxbozyx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tmslhvrc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tqdodhzj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tidxeqsr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kvytpbhy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xflxxzyh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nujjbxlh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3upybgoeo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zgrtzizj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rgynkrcg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ozitmfwd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ejoqlget.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqnblioe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rrhitgwb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qvtatlib.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bqbcyfvp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kyitmszq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ntuhrvcb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pdbfmiuk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ionruhnt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ftmqsspv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fdkcteta.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cssmspyk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3safnywpv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bttrihuc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3behnkjng.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3onassllp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ubwzbwtr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nciezase.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tpjwpcmc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zxgrtjbq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oixlfqwf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3swzhnjie.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3izdwciii.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aagpocjs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sjpwgcan.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3twlmpihk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3doctdldg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tyfxgdkb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3miziifaz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wpxcotrz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wqpcoqgb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lhvhzigz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xjxmxmyq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xcidlrzj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yizfcprf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbftdjb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qnmjhsyk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3orabrppl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vplcztas.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xyrigadb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3giedxkol.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbarygqd.html


<!-- 参考信息 -->