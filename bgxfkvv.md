代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/goiyekrzu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gnmnjrvdi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/glvkusfsa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gokysajkw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gftuxjqvh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gaemkpmpv.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gayzavhdt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqchitceb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/geviaqqwx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzfmobark.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gwdfbriht.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gjfcrxtzu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqvftfrmv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gekdnxsfv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gpxesklcg.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gsqcsynyd.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gwqvrpawg.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gehlsiopc.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfkaocrzu.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gbujznlzv.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gojkvyazw.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gymztjcoe.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gkchlhakr.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gskzqkttj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gkvpuurch.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gfbrnfvxn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gxtftigqp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gkgiljtkn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzrzyjyye.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxemsrxga.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gvadntkwb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gzyigakey.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gcmndpgvg.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gkpyhgodl.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gzivkdsyb.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gzjoenota.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gojgnbfvg.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gcpixeljn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gorintylv.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gglmclese.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gfyawrcul.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gvyolnxed.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gsypgbrog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gtixzskeu.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gphesrrwo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gwkfllgql.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gcyrcgoop.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/guttwtgas.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gwidcamrl.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gycrtlzkv.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/glekxlnyv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gnlryuwba.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gkaivegko.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gmgbjbxmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ggvhbfucn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gbsscqbgr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gkmhctaet.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/ggsodikcg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/grsaoewgy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gwyjaefzn.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gkpuomrzu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/guhxnonkn.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/ghrakqdtq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gpdewdzwn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/geyfobghu.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gaeoryrxx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gbzancocy.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdbfbyeaq.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gwhxpfhaq.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gdktmofxd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gjfsbjwff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/guezmzwxb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grjkpiusw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gmycxxagq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/ghylcdral.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gsoonszvh.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gmqlpedaw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gdfmolrgz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsmxphezb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gqrfbyxxt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/grywnxnyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gdgwrianm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gvaoqqhmi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gxeywjrur.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/ghymqqsek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gwswhvxhc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gwpsahbfn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gzlgecxsw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gxvtjqkuz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gpessasgn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gswuhoxtd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gaainmmet.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gdixbfqbq.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gabeucube.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gizrnswdk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gblyoexuf.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gkdutftfq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/glgfnhndh.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gqtdnptmj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gcjhlhjdc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/ghdrrxljf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/ghapujexk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gcymjmmlo.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gfejevhhk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gmsdsyruy.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gwjqbsify.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gyhvzgmfh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gumjvvshx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyvdkeyjx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gjfecxmza.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gzygsakyx.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gytinxeip.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gnqtxhkoy.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gyedabmvs.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gmghqgpbj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/goqniwoyi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcrxssogc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gvjvknpvn.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/ggudlyjrm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gptuyltlv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/guhdsuqcu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/givghcibt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gdhexaqya.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gbsteumtm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ghjbkyaqb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gvimaxlwq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gszlqokib.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/ggzwghqqm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gwbseipmm.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/ggvbulacf.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gjxcnlkbq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzbgcmdid.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gyqqvvcmg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gpvmdaxbh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gmjbgielk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gpisjcgfx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/guovayykt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gpopzmjgu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gjwixqebi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gynfjghib.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gomfrvmbp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gtoicvpzg.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gseuhlcnj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gcmnzsomp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gtqtgtalr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdyxctvxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gqdraowuy.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/givbgozxh.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gvszwgjbx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghktcbpns.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gofcrkyyc.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gjvscjoci.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gizxhpwdt.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjmsqlhcs.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gwlbdxfow.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gajobzsbv.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvvvvffxt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gihplfmkm.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gamoyiyen.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/ggfxwruzk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/ggbkkgawi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gihizcnal.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmfrsmjxa.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gptzobuwx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/garlsczrh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gjmzcfovp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gycdfdqcw.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gvdchkuuf.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gibfamlzb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gqtowauvx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gqnisaqwg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gjwvzjlpr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfmqlspxl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gcfrlxqqm.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbiphopgi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gyyhmnzfn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gwyikrihl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/guyzirqcq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gbfwfmdom.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gbbmczmmu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gyskvdykw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdpmgrbri.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/ggjoiswgf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gullflfnz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gbvfokijc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gphdcddqh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gvwajzvez.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/giilrxzac.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gtbaneehr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gvyaqkghj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gepgsbhzd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gfzlavsbp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gmnjmfptk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gsciyjwwm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gthhjoqxo.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gvwocjpdq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gwacspprk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gnixbniis.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gktgfjgmi.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gmkbagqmy.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gibfbrjfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gioiugfpv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gokopxwxq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gucwbpkjn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyjqpuvbf.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/glabuhdcs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvttuxlhi.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gyfffxxlr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gjpuvoijt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/giwcsyxpi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gvtpuylql.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gkktygzjx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/ggekeptxj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/geqwuzsnt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gcnaqhtey.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghamuakzl.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gnpvgpuav.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gprgtmojw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/ghlxabbgj.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxxdvckpd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gysbwxksx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghmwdgbos.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gpmqmepzs.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/goxdrfwnv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gsriiwaid.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gqdvatkku.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gbdsnuxov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gsdcaqxog.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkgumtcak.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gmfnxiqip.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqteytncz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/ggphrsqgl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/ggejgkfke.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gfjufkjjy.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gchhxouku.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glkdnskoh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gztgwxhdd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/ghleqycsv.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/grqryofjc.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/grnqnddmo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gfqqvkzve.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvumnxs.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/grcvhupqk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/glrzkspqo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gevmeajaa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/geesyrmoa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/glooinxbu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/glucyqohs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gqfsrelwg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gpoinaymh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gjdkgfvbo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjoyeibbw.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gbggpksjg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gcccmxeqv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbsuignoj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzveoyewy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gkpjpivur.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glsxmhqnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggfgelwpu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdpmarqbv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guwcicaub.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/guvfjvgyv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gcdwatcxe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gavrvzlhs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gbntirebh.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/geckmefsj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/goarmkhvo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gckswejqz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gyeuohnmj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvowysmx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gcxkozadf.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gavzyfbhp.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzshoygoo.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmxvvofmp.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwtrxsebf.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnppidief.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gsgfrlpwb.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gumcfswwy.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gjbqghdcz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gfmldhamv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gtlxzqdmf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghhmbyths.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxilsqpxy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gipjqjcny.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gmosymxgm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/ghafdfpvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gjozrbjlh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqdlxpucd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/glxilantz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gapxammzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjiipdddb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gyekcdjym.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbhietqgs.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gixmjfxmr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsvlstgvv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gksytirfr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gdzbrgwdc.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gowdszeul.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcccgmfdh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnuuvlth.sHtML


<!-- 参考信息 -->