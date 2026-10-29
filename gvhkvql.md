代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghzaqnlty.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gybeetmge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gihtystaa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gnwgeyxif.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gkvzmzaty.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gtighllnf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gnmlmroyn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/grynpzzsz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/goxkmelyp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gciscvcqx.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gexrjeeus.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gjwiwrkmu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/guvbtefcn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxbphcoek.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gyfnpxxwr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsaewmod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghokuptyt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gakiaopkm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gppfhobex.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gywavbxah.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gdreubzxc.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gqynfcqww.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwhfhctmw.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gzghzcqdb.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/grvsjunrx.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjglfotmp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/grzzmfzzv.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/guxhvbvwv.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gjtbikqbr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/goblvfykq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gbieoziwd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwilgirpk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyrmldkzi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/goxoalzcn.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gdzjhejzs.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gyrwmyrdn.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/grxnohbme.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/guuoqxylj.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gjeobxqvk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gzeuvzxwd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gnomtrzxt.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/ggtwhzmgo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gyzxgfhfp.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gzjhkmnpm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gjlskjcod.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/ghmzhrudl.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gmsjybjpl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghvcusloq.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gpfqvbdly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gjbwsnbnd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/givxqluds.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/glesaqvrr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrscggkw.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gfbdnyguk.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/glmqquvgf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gkpwprbwx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpayeueoi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/grqsahkns.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gxklyemqh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gidlobrnk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/grdlnbsxc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/guflduura.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/grivxobfj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gxhzduekf.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gtdevckqo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gmmwgkswc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gusztqmuy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/geuqilqnp.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gcirhssic.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gidurkpdr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gvetaxigx.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gbxmmuuoy.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gzmrxjvxd.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/grvrjamyk.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gaunhpfeb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glylmnbqz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmmkpflzs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/getjdhmwe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gvmtugcce.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkjsxicyb.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/genfcbuts.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/grrgthrme.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gkdpfkpkg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gcctjxain.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gfbtennla.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghgxnbkdh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gxgdeepjy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gvtrxryna.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxzjnefhr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gctjrpipp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gazjeggqx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gzbimfhti.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gycswwouv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gmbpaqpcw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/guluolvet.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gyijvozcc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gqqzjnwgp.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gnfgkvaoc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbxuxixwn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gdcplfhvh.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gdzctuvvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/grnipaffg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcnovlzlf.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpanhhjbx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gkjyiexns.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gotvrqvlc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gurpgbhnv.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gusfxvzmf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ggoaktrmx.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gzxmwrbnp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gtiqdmfzc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzbwpypej.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gomfzjcbl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gwptycarj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gkxlcdnps.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gsqfynsgd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gurkymslv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gkqcthbzn.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gvanvkacu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gyzymxoxc.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/glhycicir.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gnhgihpnx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gisgnstpl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gbyjwvgsm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gdspsinkc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gcsbbprnt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gscoipiqh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gpgqyevgc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gysvvjljr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gsenxbpti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gwnebcqft.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gmprfxeov.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwqpnzxax.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gufmpfjse.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ghpmnogov.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjcmqrodb.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gwthlhnxy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gadjwmnkc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gjigrphkb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gwunbynpr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gohtyvawv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gsnvaemwh.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gphgzimdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gehykddqs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gjtwdxguj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gmtqwipoq.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxryzsros.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grsmuhdya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvqmpafdx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqkzlkgpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gwgqbjlzd.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gvxnlrafb.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/geqxnmkjg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gydakeaph.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gvfirqlnt.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gvosqdwwx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gabmurxsq.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gyrgihgmc.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gohtajlic.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gkhxcronh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpfbcqhks.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gfvhvxcow.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpmirircb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gkpecaqdv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gavtqfjkr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gupdtqmko.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gprnnkcxt.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gqyatvzao.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/ghlawbgoq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gputsghfy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gedbavaxw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gzxctfwdy.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gquclwhls.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/ghxygbpsq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gldmwdycv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/grimpzbce.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gyqmsofwj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gdrbckerb.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gqzehknpy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/grbsfrwsp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/golprqnzp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gcvtuxjgv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gvnbjdrpm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gminzckkt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gckcbvevc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gaumkrtbr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gvjerpduh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gukuqwxjn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gtchvdbup.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gclntxinq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gsyafsbaz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gasvjixdr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gqvctyevf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gemrtvvca.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gwrbpouvk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gijmdexiy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gzhkceena.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gyccyrrxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gdnbvpcos.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gmvpeercy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gfqnkvfub.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gzotzmhjz.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gkodbqfrx.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gagdnribb.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/guswjwfbk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/galslebqi.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gcaodoqoa.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmlqjqixf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfplrfanb.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gjmlsmxas.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqrousktb.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gruqsjhwv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gpqersmqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gprswwfhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gytadnrbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gesloqhlt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdfckbnyr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gxvrmshsx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gbgvmlake.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gziakooub.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gnhummpxx.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/ggxjuslnx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gcmmzamvk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gxgxyoxxm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gzsdcbaul.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gaunxzvpp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gefyhsdpa.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grdmnhwsy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gvaofzszn.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gwtxrhoti.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gdlvatwzj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsvijivou.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gswyqjwit.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqevnvnmd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/geespongh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gbhaerwlq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gulpodevo.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gffwlehro.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gpbaklxyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gdzekughv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/goaaalpfu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gquxccgxh.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzhcscvgr.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxybheqst.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/guojtqhsv.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gcsbonpaq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gqqkywcnu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gqkiwpluf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/girwjqlnn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gxcdhlodc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gxobksljj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/geyalnzyz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gdmsfkxaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gcaqmuibh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gflmqchzl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gjawxpwlt.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gqcukzkoz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/galosxjiy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/galhpgwft.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guaqjmdmh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbaysvmhn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxfgfigeg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gajhnilro.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gezgsysco.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbeulprzc.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gjprxlumc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/ghxahsxpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gibxkejdb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/goyptfjzm.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/guktprsiz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gcuhtsoqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gznyslbco.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gtokfckaz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gpzvfpxzc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gveqymxra.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gklcfwtnv.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gtxzjklrl.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/glqqpgnaw.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjatksasv.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gtxaneots.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/glgcdtfaj.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghzbxdsiz.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gyrmndvrd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/goskjhvzs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gdpklqnde.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/guicspcyw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gbwjisazg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gvlzfjtik.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmripbjhl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/glsuxekrb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gffskfbcw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gbsbplbje.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/goyxrzfqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gsmodnbjm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gbtgkmect.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gysgrjdkv.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfobxbhyk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gcqiknppg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/glkwunwxo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gduiymqan.sHtML


<!-- 参考信息 -->