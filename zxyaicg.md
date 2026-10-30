代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzvwnewtm.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxtzwrgte.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/grnirdczp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gympxopvh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwedwcoyl.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gfqniuucz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gwstvmlha.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpbxryrrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gtndaanij.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gkjctarph.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gnmefkmwk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gonbhqscg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gkkqrhuvf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gzzlchxkl.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gjupgkpsa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/grkkslxwh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gijhlwtfz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqehrzghe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gsxmgejtj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gysorgznx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glyvmonfn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gifexxtxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/grjpnmwaa.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gszsslclr.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gzdsviwci.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfpgbgkdj.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/guvwzrmhd.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gesvzcmhf.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gqmgwpyan.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gpexledue.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gzcyyrokc.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/grvcfprrn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gcyptmror.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gbslmkuud.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwdtfkfnt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjxaiprvz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/glcqtaedb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gblzbqvdx.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gencineuh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gkpdwsbme.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gyzgfcppb.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gqrctxmqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ghnsbfgsz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfufzgt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/goivhijrn.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gozzwisyq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gueicrirt.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gkvslhxmc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gebupatqt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbibxdaoi.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gmyrkwavj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gpsnymcix.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmwpqzrky.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gzcctpidq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gcnqfqjke.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gaxnnqwnh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gbdtsniva.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gprtdstfo.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/guzmdhypy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gydmxnhjh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gjkjjzwog.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gsqaujxgn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gwbdgjqhd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gxpuhuvjv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/ggdykhfen.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gcsmjvmza.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gefzaubnj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/glyfnodzc.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/goxinlouc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/glvjxezzh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gkhvsmqdd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gseqpbbce.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gxzjyalby.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gxqnzsuhd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gudljyfgn.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gztqrdbva.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gittwfaea.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gjpmupbge.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gqnplusui.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/getybetro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gzzzlqlra.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gxgkskzzc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqiyyij.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmeahipmh.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gukfuaznh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gwpvsjlic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gqsvwcmfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gaeyigpis.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gqudjtnjt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gisrwsbaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gizmyazgc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gsmsqoggx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gyvpravpw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gnmegmhuj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghipfexdp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gkijswdhl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gjijidlgw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/getlvgeaz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmrctegqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmiazzaux.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gpqjqscls.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gcrccykgv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gueborvjy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gybbrgste.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gwwqbydiu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gvubxgpud.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gycckvxzy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gfoptjjuk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/giqipyfad.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gbrtgxnsz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gcnokidvv.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ggsnbsdqa.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gehckhzrh.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gamgswglo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gjhwqrklu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gdbiuyixg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ghugapnni.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/guczttldw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gfhkfutos.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gyffmkxkk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gebzftpds.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gokuwlwpl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmkarlobo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaybbugem.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gvwcczlzj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gnjqksbny.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gfobqwkvm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gijqobhfe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gftcgkwmd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gioaexoud.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gqtmvpqyd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gwmkbvpah.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gmnzlcarp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/ghlolfjem.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gcsrjpxzg.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gpbqsyvsb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdmhfhokt.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gbelyamxc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gmsgjfnhp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnrxlkeny.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gwfvmyxrf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/grccnuqlf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gflmhfzzw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gdrwmkont.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gnornwimp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gmwjmprzs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gduyvwlpu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gttecajdk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gartrkops.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gkuykcocs.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjxlqdehq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbihrwofb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gqunjlqig.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gkidefgep.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gstcbmhsk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gtcdtmxas.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gvpzmzmkv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/glsziimhm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/ghytbjmeh.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gzvuvclon.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/ggnvywhyb.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmscaxyjz.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gzkqhrdcq.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gvzvruedh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/glkmwjaad.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gozklqzpg.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbwmxnrem.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gqkeyueik.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gsmyedwne.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gyttvgslg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gwqkvyrvo.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gaxahffit.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/grlbgupeb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gtriazqrs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/ghbrrgkjs.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gvqqltkmi.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gbhsdabsf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gpidabykl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gyfcvzehy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gpyjvikhc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpebnyoqk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/ghuvrosjx.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gbdxyjhdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gcgjnahyr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gejxlehvd.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gdbmxleqv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gpzidmnvo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/geayznhxn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/grzsbmhiq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/grwnkcgqm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/ghgvnjhuj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/guvbhygsg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gdiowyotp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/giegbmlpy.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gptvbrexc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gyjvdevrl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gluuvcfiy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gcldqyary.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gqlehjsgv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gcbvclgwz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gcoibrbdl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gqhjuaabj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gffnkcazt.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbbdanqnh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/ggxdgybkb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/galnqoajg.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxynzskmc.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdshytajs.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/grrohjyyt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gywhgruox.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqvmoahho.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/ghtfeewsf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkdrukhxw.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gyvvmoxjw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gitwdjhaj.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghyefaqqs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/ggqazivta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gndwcecdx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gigzwfdvx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gatjvyhim.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gbabkilrt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gjogxcusq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gghhyyxtz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvenxpxqd.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/ggxokgafe.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gyzzrootg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gpimmlnui.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gaternodj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gnmvvupog.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjxmqrotw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/ggkqibygr.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/geblxkuun.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gmrszkicz.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gbaxbvavg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gfdelwjtj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gafhplfvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gwxixhkyt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gtlzlraai.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzgksfrja.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gtyzjphpc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/glfwkxwqm.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gljgwlivw.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gdmgsghhq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gpyrgydkp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gmibdulmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gyurwgbga.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtnubhylg.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gsfvrfwgk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/ggdnhhdnz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfsttrdcd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrqgbdyn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gzgtlsebp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/ggifmcvjp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/grwrxkoay.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gykipjmkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gclhlwqyo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gcoljzdbn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gnxdsbujf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gvgaputgo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gvbfpegoi.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/glkdirfsh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmqcrjaxl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gnjfszqns.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gscxbzfou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcgeqeize.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqphurwcl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gimstzqhm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbzcptqsl.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gufzlooxy.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxoabdeiq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gjwtmwllr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtzgermkg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gzjwghglk.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/ghytshiho.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gfegvxgme.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gyjjcpdim.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gwrfoznbg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gmcoonjup.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gwgvtvttz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gflahubof.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gqvmccfil.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gvqubdhtn.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gjajnfoyk.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gsjotnyoa.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gvtqhlscu.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfmmofbsv.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/ggrvikgxh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gucvqegud.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gdabkmryb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gvvioezmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gusgzshrt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gmcbynxgl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gfscobwsx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/glyloinpd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gsjiocfaw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gymhxgfld.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gjatvnyah.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gelyhwcph.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gpcvmilis.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gzwkjxbwc.sHtML


<!-- 参考信息 -->