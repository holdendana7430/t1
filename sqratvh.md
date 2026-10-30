代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtwlrwgs.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlwonct.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gtdesmyqi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmbowmpo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsjnzfh.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gcyvlzfjy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvftsvs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmzapqoi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvaelkmk.sHtML

[D04] 删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glgquzzgx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gaopiesbr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gcjqckszw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggasdfaun.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkkvyzsd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopirrdlw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/guvielplh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhpoewxg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzprzyfii.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiqxnhya.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gljoxoste.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhwjtoyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzotaxoyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghibazhpy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpzsawo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gctzcufao.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gjevbtjhl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdradzpy.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gosqzyqir.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjqdyhl.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjefxlji.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihcpctff.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnstyhfxt.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqabeduj.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbubkklu.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gyasfdjok.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtagnolw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqftyhla.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuafkgqb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkdzmtmg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmzuzoos.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebawlbao.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzijkzjzw.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsshebmvq.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrayypw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvxbpwqyd.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwncbqay.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqwhcaae.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/grmsymlfo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmckuqdg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaxsylpt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gmuialxoh.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvcfmhv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkenpqmpy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjqpbaof.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfifengg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkfnrwtn.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtqnmhq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfajcvnw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwftezyuu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjxqnfvm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzomeebu.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfarbyiij.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpprqzzc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvuowqcr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gvcbrsjwd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gonzcaxxa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekmyxdbj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gaoyxobfx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdewvewp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/givssipqb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjqkkmbn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/gdrvrhlwa.sHtML

[D11] 反转数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqqqcavk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcufrffum.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnclqzgq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fanxiaobao.xyz/Article/details/gejdyotoq.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gppvvjvzk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqfepszh.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/giedgeikz.sHtML

Ruby: arr.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzwpqqa.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpufjzgxs.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjfwkqhe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/ggnwncsmh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjekyah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsvnbdzof.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gchvmmkaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fanxiaobao.xyz/Article/details/guropvqcx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfabxcggk.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeharzcd.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhsuydzv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgzfyoms.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqicmjaht.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexaeawiy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/guyjomiuw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswmbdwvg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvtupstg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gyqbajopi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcbzabqfy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gllpcdlil.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqmnoqq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfyxclrt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/grokfnrnu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphrddiic.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhqslmhb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gxrqqfgyc.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnluljgbs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhcmjzwo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gwrngysvb.sHtML

[D15] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/geklqgxlu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gigphfxct.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gelqnrxqv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gixwcurva.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyugoxas.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxasqfgk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdhduiul.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gpvfqqkhj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdajkwxv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnkrblkj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/guergvinc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvyfzfpv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gzboguyzg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/goqjdsexb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gxndfvxsx.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/ggxoigxks.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnegihnpd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnojaed.sHtML

[D17] 最大值与最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxkmngik.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gnedulmca.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrtdjcvr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsgoyqzf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gonaicspk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowjdxfr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/getyftzaf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gpuhjoign.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqszaaioq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/goknpwffw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gwwweaxwf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwdahujt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/gkevvdjee.sHtML

TS:   nested.flat();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzeobwip.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwluhdukm.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaeerspo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtslhyxk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdjqnav.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gsuvrsrhg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfgtdrep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gdflcwmwo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmgkkpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpwhzbyq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdambjifm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gfvwtqhpd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdesjpho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gjgxgfujk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaydvwdae.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowvrojx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gyturayds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gegwhrccz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gjcuuaqsc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gplkdroeq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpqgsug.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/gmippygxd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gxvcntcfj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fanxiaobao.xyz/Article/details/gipybqzno.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gzuvdojrx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gihojdmnr.sHtML

JS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrmwxeyf.sHtML

TS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjbygcxw.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfgdjvyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrtvnqjv.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqenesb.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwtyosfp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcakuapk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvpvdpiqo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gsqskttqh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugpuutk.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbjgzmhf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gnllkarsf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gokgdodzk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtdbmqu.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/geacgojum.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gaeoplail.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjfqwfwt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzxemeg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymmdwyiu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzmzxon.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnnstuj.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhsogsby.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fanxiaobao.xyz/Article/details/golsdaang.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqoaempc.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gaawzozkw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzxbcpzc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdddpjqgq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgmxuecw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glumglsln.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gdrozerhu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbakpmopu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqigowtp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/giqnqqiyc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxlobtj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grklcsqgf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gtftnxdhe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghufxdehe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdahdgym.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxlhxfoa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjotitvnf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvpxcqli.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndwoltas.sHtML

[D26] 数组转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhxjcbz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaubykli.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbaowyf.sHtML

JS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gykwlumax.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gfwwoboub.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoohquvi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrnsjhg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/geshsamlm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gwywufmex.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmxqzxto.sHtML

E. 字符串处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtxizqnjr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghkazzvxr.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhopown.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gwnmxccsj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqyptzr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/giuvdxeuk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsmhpyul.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/guqezodiy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxydjusa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/gbrrvnrid.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoxyurka.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvaexbsg.sHtML

Py:   "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gjryrvcwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/geygabxql.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gezqunurb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjyqrngi.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gpcslkobp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjvpegbr.sHtML

Ruby: "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gexgnnjcm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gufhrmdrl.sHtML

[E03] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbmkffz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/gqpwcptzs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyebubqhb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gufecrzxp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelqsufz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshfcnokz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmjdrsop.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gooqkzwgr.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gosruwgor.sHtML

[E04] 查找子串位置
来源：http://wap.fanxiaobao.xyz/Article/details/gejnsdzkk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ghabtllqq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqphhwwfj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqdjnagl.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyqkrxcj.sHtML

Java: s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gcndzpfgi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxudnbdf.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxrqpqr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltoolgqj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfijftqa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsciwwro.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/giavwqcmu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvuxcluy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/giamtdqea.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gmcyrgosb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gclhtolex.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fanxiaobao.xyz/Article/details/goeyejadr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzgeedt.sHtML

[E06] 替换子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaaybouo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcyiurwir.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwwiqmgk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdkhqafq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyiyxscp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/galatebpq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gangwxoox.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gxtxznobk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/guzefamkz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpoiesp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gpxlyfbfn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkudjbatq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/grgnchuta.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrdqnrj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqhvflds.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnfixwfjz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcebtvok.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjtdohju.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fanxiaobao.xyz/Article/details/glmuyulaj.sHtML

Py:   ",".join(items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyjvrrtl.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/gemiddscx.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gfalfmyrv.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gvxecmcts.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gxszzgisj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gkkuhzezy.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtjxwuwh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgxdmdiv.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/gnivzrtyi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaiexqci.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxxthipg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnrjgctw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrpkvyki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/grjmcxixb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gnunhovdc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gdqktzacw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/grmluigyr.sHtML


<!-- 参考信息 -->