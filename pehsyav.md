代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gayjvxuti.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnwaopyds.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gkkpuqryn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gyymflkul.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gkzdlssma.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gstumoxdu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/guosoowgd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxxxffjvh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gitvigfgd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gpmitrogd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/goftuotms.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gastvpfry.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gfibjwbhl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gbcwiozkp.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gpfvbmjty.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbnnjfpxv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gsugmampn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gazdgydjh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gpvcwudlg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gxqiukqnh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqrewmxkb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gzpgobaau.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/guwzmxkpb.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gbnbzjtmj.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfmstftoq.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gjxkwrasq.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gatjcvrku.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gjmkqbafw.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gurpwzmch.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzpjvjboi.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghbwoyssz.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gqlkynxvq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gygmbhmnd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gmawjzuer.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/goqkhaeff.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gycvgqbhw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxkvbnhgp.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/goolidekr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gbvtappfl.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gkeoefffc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnzzwexfr.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gtwefbmdr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gbskfmxvq.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjflaliuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gzynaizoo.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gakfzbajq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/ggkliesgt.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gfphbxlfm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gogahjfyl.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwwdwbilw.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gbjdhacmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfgnqbbsp.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gaazzlqqz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gdwuevcly.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gtjknjvgj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gokdjcogb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glkyrlhuc.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gawkfbeor.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/godytmhrj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/ghxafmyix.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gtqpmscbu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grtnalcob.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/ghoaxrmrm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gsaobwtkh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gukwtkyyg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/grrcomzhf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gstmyyvke.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gjwjwjddo.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gqsltwmju.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gnqvksyfv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyeojatsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gpinyjjax.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gycuqnsze.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/glddpjate.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gktffjspq.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gqrhmupfw.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gjfasqdqd.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gcneslpuw.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gwqitfyym.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/ghcikwmqi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gtqxdgvxj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/geicwmxzy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gnzowvvau.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjhrefmtl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gwhjhzroy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gshqhsywf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gahdmwybb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gxeftvrqx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/guiwplrvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gljgvejqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gamobqxzh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gqufloeka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gakxgtuff.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gipfgmtqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdogtiick.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/ghhlrblxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/grnewrzdv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gwyypidvf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gepkqzmxb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gcovtjnmv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gsjltscrv.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/giqodkljf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggvimqzlb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gatbzsgwj.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/ghnmiolif.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gakvaebwo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/glqoadpxa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gkxokcyiu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gwzxumnzk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/grscnyptl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gsswbvkyy.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gbihfqash.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gipqoqmcc.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gmjxnsrnj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmaydpwcg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gakwmssay.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfjfrmuls.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gmukccmyf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gvvkpmnxr.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gcvsfqptg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gatjqiyrn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gpsbmsmvu.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/ghrrmgdnd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gdawccbmk.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gpcoiacav.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/ghqazcjyy.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gkbxyyuiw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gpyhghczu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/glpeomtix.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/groojdhjg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gmcnrpfgl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/grolnjoez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gkxdgpxrb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gfovkhvnt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/ggndzcjrg.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gzjujblfi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/ghqqqlymn.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gnoyfjdck.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gackdjfpr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gnblwqfvv.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gvuxbnyct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gdntarpie.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/greapzqxh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/guixifsid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gkouscmbm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gztxvuhmc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gndrgnxlb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ghqplzqfn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gjnzvxevr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gzjljrifq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbwlivcxo.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwnbvhcnn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gnqpqfoav.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/ghvscocgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/glkvjoiub.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/glgzeqaas.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gyvkaseex.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/ggemsgtir.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gfoqpftma.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gjrsyuftg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gtbktwdzq.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gcduziixh.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gddqvddpq.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/guazxnhow.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwykazxyw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gyanxqeux.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gjnwigray.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gaucagtkq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gkdgbmkjb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gqswgxkxi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gchjyyxqe.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gddifzmdy.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gnziaiujr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gjoosaixc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gmctlewve.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gdntmlroy.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gnlafgtgu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gxrlnlgpi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gcumbbetf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwnumgnjf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gglztgnop.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gmudlltms.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gpzrwavgd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gkagdflwc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gvsgfzhwt.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gqunkynrr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gxzkywjxx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqdyrdkma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdfpskarq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvminkiaz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gwojmiedz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gilbljivx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gcgysqsrn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gcsrdkcqz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gydppergd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gxvqjhifb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gsuvwurax.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/ghahhihkt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gbmysbfeb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gdvclpack.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ghllbfnnj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gbwfyeywr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gtgokznsf.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ggtbmmrfs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gsaklxecr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmikmsbmw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/ggdrkhczi.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gyeezfiwj.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gporcnflx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gjpgsdabm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcwujqnis.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjvoopsaw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfszzamaz.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/giiedxrfu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjfbznu.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzhgotxha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gdtozzftc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gjgktcamx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghuagupkx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gchpjazcu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpyyijojf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gcuvyjwdj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gpavlidne.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/grjvxavsp.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/ggauxzsbc.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gslmrsrov.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvhqnxvht.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gpujbscrn.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvpumdxxz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gadwhtncd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gbrusfbwf.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gizgpmxxn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gtgfnaumt.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gbxwilhzh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gqdegpujj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjsqrlnqi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gfkgbflaa.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gftwkqsyk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbuwwkzfd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/grbtyivdr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ggohowgpz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gdlrektuq.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gnbtkmbbt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkpbbkqqu.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gggszbkud.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gbktbfrqc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gaizlzkjv.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzbxoumey.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gmkmcseti.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gnghweiup.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/glvsslbrf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gudmrjuct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbtbijajh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gnrfkttmf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gtabradxx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gjzfmxeui.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdbmxpkyy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gljviveiu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gdltumain.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gcavdkdqt.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gulziktqi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gkbdfyurh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gtmytjrul.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjmvjofpu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkobinkrr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/givfomgjz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gjtzbhift.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcfnphfwm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ggdcqzslq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gjfsypjqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gjmstjnjq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwiwnxode.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gubrhaoqu.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqfgjqxlf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gnfjnblqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gfqxagjda.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/giegcvpjd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gxabhknkr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gjqzkthiw.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gpfyorhdn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gbojobjux.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkdojypas.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdxvdypap.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/grprqovfu.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gxucnumxp.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/ghqntadxp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gqnfmpixp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gbgtkllib.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzhbrijqi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gmxzqnrky.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/glclabzwr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdotrxho.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ghcmdotnz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gngfabnhb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gcgemwmmd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gagchuwuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/ghlltvbam.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxylrjzvx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gmtyhtokx.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/grdiwuoxt.sHtML


<!-- 参考信息 -->