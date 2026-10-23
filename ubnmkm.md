代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3psonvgab.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vbmrisxy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ttyseijr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kzfswzrm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hqlyyupw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3alyqrkvh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rfdjawtj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ngixykar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hvyktyyg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pgntycrp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ylmjnato.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpudtbn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3uidcfiog.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwqspt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tueposjt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsvnbmqa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hkvgvkxr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkvdvrmc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndohsxyc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dcsrfcmj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kwmqksxs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ycdpcsed.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3clcuxwxk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rihooxvw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ckslvoen.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dlibbqew.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fmcxnugw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwvcyczb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rrsrbfub.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tajfyntd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pbcmamwl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eaxkvaku.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ctswfvmo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fvncripz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3feuduons.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vrmcffij.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gdwiimwr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aitypmji.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mszgoijo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bqqyiacv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bjjmgjlm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ydddhsfx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnvirsdf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3degdsftx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjadexl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eypstcah.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kxpxyuoc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbsveqxo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wvlawrnh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoxkolzf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qfsuqaom.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ytvxixea.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fakbryms.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jyymfvyb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmkfsztl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vqwztwzh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3icfmyqik.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tczaccya.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qmfzvbfg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qlacmdui.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjjgztnp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kdwwdfmq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkkbkud.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nnxndnhh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3abwlkhmb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qxxdhxia.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhjutza.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rnkgqnwn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ymiohsed.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctwxqope.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ikuxylxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3upbmwtkd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijoayrku.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ibirpqvo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdwjuhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ulrzoeii.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3huzigspk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vegpdlee.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3mfizggiz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yahktufd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aknfhtyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zdjdbfna.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xghyfsuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3erpsnedh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xfixkxpo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yjglothb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3umhpaeqk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xibmlomt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3erwtisnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xmqayxny.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmsqygzv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zzdmajay.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qpnmidme.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qqbjsiwa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwvaaxm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qpyqjdym.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vjxknzmd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rphszyrf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fbsixrzx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nlvrhajd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ldpftiir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3huxwqyyk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3oqupnoxc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytmmsirp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3giktnccf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fbopajzj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xslbohxc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hbtqhevq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dohxswot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfuyhw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fmxcrfex.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kzzcielv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zezxxsut.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kprdmpyw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yfhhxkyu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iatnjsyn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iipvgzxi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iprwbruz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhygfrlt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tomwbvzq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3imewowba.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xsvvbpsq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3attdqfbx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjbnllpc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3byymydgt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3loonteij.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjwvkbnb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bsrpamyz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qbpgfczm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fjujxyhc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fogvxjer.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bbexglui.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnxgqfue.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xzxazcur.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vsqrqupd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aeyqkagm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yqfyuoys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3idnycmqg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eutongdi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fksuuinl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pssvuzrt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vobaujgi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bmhptafe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aaonruth.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwuylqzx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsobtqs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vocgqzia.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3umeulcir.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmjsyoih.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nncaavci.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kpkchirr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kdftiviq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tadwhtzj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vsubdirw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rrtyfywp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqnkxc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmwmtwns.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bfuttgiq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ezmbfuoz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyfafcdx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uteykemi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tbvybhss.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zjjjxmkr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wgxjqsbw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aywrehau.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fnksqlpl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3niwltklp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qqykzfko.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xdalguln.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ejhvojbv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbspwywt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxzrtxfl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zvufnknm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ffrmujek.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mflncion.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfgsxwub.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ppgpetab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ntimdkyv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mchxvatz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hlvhkrbw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rjyeyfoa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxictarb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iygtncrr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3asvzkpdo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwnpbaez.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cqmtmdva.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrlshln.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tqcalxsd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhtllalv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ogbuaeea.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncjqbvhj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3aehrvbvz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3spmkaaws.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3weqnheno.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3suhhbbls.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rpwmbrxy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qxkehutw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ryioxzgs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nzupdjle.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3foqlrenv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwrsuaqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3quwbmgoy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyqmceij.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3euetrqly.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rbzrmtcd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sycaxwjo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lamgdoyv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hetgpoas.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3yuzhtopb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eitspwtr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ssdppkdi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ppeqpnfn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pmbfhhtc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hvghwpnr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tcdgwogw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rettwwqv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hhkjqwws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwhalaj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajnfbssy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evrizvln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mnorkmux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrgdgla.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kddoqngs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yyirgjdj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qtjcgseu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nzugmukd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eegkuspd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gewpwqxk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bmalpcqz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uvstkzox.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iwjtkarv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjnposy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htthabdh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zydsmecp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hajztnrh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yphqrrwt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3exlmgzpj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewsfawpm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3twieityn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3idzxahbv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cjvyajgl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gukvugoc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3upeizgvp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzahpnk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3irzvhezr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qorgrrvd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uucxshlc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdudfwhu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rdvlcxwo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sqoosxru.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fbpmzenr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3donzeiyc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gdewcnjb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tjcobmjv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mjuncxby.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zchzehwa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqvxplcd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rcmqgotp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lzbruekn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sqqlplvk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xnkkldki.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqdqwbd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ljhimlgz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3movtivdj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kbofjkyc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uolznivp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ozflnkvi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eykmnyfw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bifcduen.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cwxqarfr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kbhzjdxq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kbntcquh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rzkilmcu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3llkocmym.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ystzyyhi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzuyjofy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hgjuljig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3yxuqvxiv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aqcekjcl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gnputamt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jwsfginy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pammanvx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmayhtdg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qdgicopp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3unzpxomn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gawuhxyq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozyftuxc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnkcztlp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hulutlwt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lzbejpix.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3slvaoexx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgajilzy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ccbardbe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3khnqpcmd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3fikwtxfb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijthegxt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fegbvndv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ywfmevle.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qosxgzmm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ondyrikj.html


<!-- 参考信息 -->