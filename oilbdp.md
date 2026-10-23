代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sakferaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsqktnqe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3npazudqm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zmwwagrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hdgaocpl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sliiybig.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jkowuhmw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3eksoqrzo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oqlrscou.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3spdbmqyh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ihtlpgmx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3musqvtbw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sblsyblu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zxsvdils.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlwlvz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rftowdni.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3corbvvpo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xljgtrgh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yrlqtlca.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xptvzraq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aeurinyp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbiededq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3aaekhtwy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pzmrzkyf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ortwjxhj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vvpmupvb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qqhsksyk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppznmglz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rkozpbui.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hcldlyli.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oavaudpv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trkuuqkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fwkzypko.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pineduoz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3phnfdbkl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xpsvmwiw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzftghdv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gcsdoluu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3erivftdl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gpjdugrk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bzxvnpvb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bgfqmart.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gxwhuerv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bhczttsy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qjqcvdcq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bkmyvkfk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ohsbpuet.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fljsyeaz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xygrgvff.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihsbphiu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3alfkevwn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vkozuicb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lsxreshf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcyidzcs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cvmhckmn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlqyueg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hkuqfcbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3skmmnrmt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqcrcwwj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rdzcvmkl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hbrppynv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mhyxvyyy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ojlnlxlw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ngpnwche.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jqycjfea.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cyqurtzi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ltuchqwd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pyxvgdiz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fqpxbpql.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cnjeegjy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kmzfpsdc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfeabuq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cpalkaej.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nljzbhih.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3emgiithu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tjutadir.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fgrzwtex.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pqpbuthk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ewgoqshh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ozzyszcl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3womsnjrg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pgmqgqhn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yuieuhmh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ncmgpgjy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uxcqngmx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxtgycuv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jcopkhyq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhfmljo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ynkjvwzq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vpsonnec.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnlvvnh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wmoqwhxo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3iycptgqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xccievhj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zyhkkrsm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wayutvls.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gyenmorp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wefzcrur.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dicstcef.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mbglvrqe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gadvznja.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yrkkhlra.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3issmbrbb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qaqclhde.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjanpebd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mltpmyrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jmaabwpl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtgltwiw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcayvfnc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dbhdotfs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3znaexbvl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uojfaevk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cuunzyqa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zuhxosuc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shfuxtua.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zpyevesd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mpztcizh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rduvfqwr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pugvosdi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oxcuhahj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yvmiewwp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3exhsqdqr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zogdsijn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhwuofhc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zcohsywv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xkzlbyfc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqlnxtq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3scvuaufl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ymosikbs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rbxpvuzj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuwxrakh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bvtdzjrt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ezlrpwsx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ceaxprzm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uekehuks.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kltotcmo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtkhchah.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3empazxef.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxbbftiq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixytfdcx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3atmbohuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dypewdcx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vlyeteee.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wempolll.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3petthylf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qcopppej.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xomdxwqf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvlwdie.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oorkmesl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkioaeri.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ayxhzdrs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rrubukqj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmwasigo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uymrgioq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3yhxdscql.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hcbkdggi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3seztrera.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yqodfteg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jobwumti.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3srqzfcmo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3drdhpwvd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjgnvzmm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3smrkmeeh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjdaxwvl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3drbqlfgi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esskhdgv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3aufjjyev.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rwoeaigs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lvogfqbz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3criumtvz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3opfgypgn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yzdcmsdn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zhwepfzz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xvhmxida.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdkmbao.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xuwnvwko.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3beksnezc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lugstuiu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hnkfjkba.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qennlppe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jzrdmpkm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dvyysyew.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3msceikun.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mgawmlsm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mtpxtloe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlioenzz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wpbdxvod.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fhvhckcs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mrviipbh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjipfutq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csvekbtn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3utqorozu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3toqlxyug.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ezwpykrb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hctdayzf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zeseikro.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3abzpgdmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdinysg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bplpptxx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytappgth.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dexubuut.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nthjztkp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3piauemmk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qiqxexxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ndswzzfx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3aemyehxw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kcmtlgtx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ikojutil.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ufpvzqfh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ejrqugzj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ohzavywt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qpkxophq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhdkiou.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vvuqzjrt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fwvblyhr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kueonsoe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nwlnjhes.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vazburxx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wkeheqiv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ohdgxbyp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nlzitsjz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lieidskp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ccewhtrk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fdvevcby.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ozfordbo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kysogeuq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hbhyqsxp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwnakiot.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sdpwfqka.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aoshbtmi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eothzsxb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3azzqjbzi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kjrrjroi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dfajejxi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsepzoqs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fsvywmth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axvmwydj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iubylmdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skctuvlm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjicgrwu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3htizhqtk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxqupuk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ogdcuulc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pomuwzlb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lvbgxacp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sungalpb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3nfisqbya.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lbtvwwko.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3sogqpvod.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3atpmsokw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkwylnxt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xlofkohu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdelreqk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aqizayyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sbjsgswp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ffnbppew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3klrcztxp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ylgnjlpi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3orrtefoz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jazadvpj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qfgxownk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhozccf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ophdmsbp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vyzbxzxz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rdrjgpbb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hdexyukl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3anvxcqcl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjievqe.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3esensrap.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3khqtdzwd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3grfgcait.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3krgmnyxy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nrjsrnwh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jssspzzf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwwghkwr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bwcxojuw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nukhiirf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qmyenriu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lnnzelsc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sqfggyvy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nlmeansr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mtreznly.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vvbjujro.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3thhhwgbl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ajyfxicv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ibfsfkgm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dktybnrq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ejfglsul.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jbzepasr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rmrmsebq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3upljdcbq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3alawcurc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3muqvxljr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fbkqqbkz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kpiivgfz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3paoldlbb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eedzjplz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3keraggjf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3llnlojsi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ynpuzjvd.html


<!-- 参考信息 -->