代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/ggjpzcwgz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ghuvyzuvg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gsufzgldb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gulficakq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gxsewwlbo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gggxhwxwn.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/ggwfscsyd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/griouzjtl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glhvjqlph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/grpfzcgbe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gzbybszqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gibwgjdfn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/goagsktdv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gagtcfnxb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gyhbxfdtp.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gqsryipfe.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gbyvdrgiz.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gytkwwqwa.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gecxvimhp.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjcbqagip.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gwblfamtq.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gntjpdvfl.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gpxgfrfyh.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gzrbdbxwi.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/ghldlloyu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gmrxoljer.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gadyrbksj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpwkvtotb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ggxlynzqi.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/grshtdmlz.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/goewahpoj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gyybmrhnd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gywefdhau.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gykxebgfg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/grkiulrzq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmvfvqecs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gnbyntpzl.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gddjyqzgn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gtdtjhroe.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/goulurfhj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gruotdsdr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmlpikjba.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gxrognucp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gfgrmgnsd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvjqmgfzp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/ghrnhkbqu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gxlhipkfe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gebvzogke.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzgziljgh.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/glibczryz.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gvkrgamvk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gegytween.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gucitrzns.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/godbwqnug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gjqpbgfip.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gjsvmozbd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gdlgwkfqm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/glvyvpogw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gwrekqfur.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gbuppkrpx.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gofbowigb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gcnflpuqu.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gvspgymyw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gzhbyvmtx.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gyeqoqbeg.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gywxihtbu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghzcvkxth.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/glvbgpyol.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gkiypwwtg.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gdqzdvopk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gtxrhwwnt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gqwitomjr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfourhv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdmxdzlzj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gwlilofow.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/goetfkunp.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gaqjycebf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/goizamzsf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/giclwvezw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gcdohegcu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhqhddx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzhmukaja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjhylmohs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gunrsltka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gvjwciexc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/ggpbirqfe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtwymafqn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gnmioyhrr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/glqqinvts.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gwlbaldpn.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gfaoontep.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gibdrjmgc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gnwcetcvn.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ganpyrabc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gionuczhg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glzrxqtpz.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gtazewmbi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gkeaensqp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gndyovzlx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/grmwkbzww.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gveixtvsc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/glcwmmlwc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gwngjpryr.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gyyiadjam.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gesdftids.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/guqscjrbp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gglfovsjj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gujufjwyk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/geusluwhs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gloafbbfb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gfmanyspf.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gzeccfcxi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gbuytluzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gxbbxumyz.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gdlnlgfjs.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gazuhcswj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gzfwhaesc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gpidezrir.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gtrhlqjws.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gbjhsvfse.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gdppjbmjd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gnvmzukfu.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gagayinyf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gijgewsrp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gpqfkzqyl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gcfzcixgf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gvwlhwojr.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gxnwmuybe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gsmhhgcde.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gttopsjow.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gdvafjunq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtecinflu.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gnquhvaso.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gvwzgyfkl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/glbiypwyq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gndkeprbe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqxzktu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gruwzupqb.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/galrklhny.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/guxaokqdx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gfhhpztiu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/guqyzbrxs.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gulxemqzv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgsafqn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/glcvycvwz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqbvozxrk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gouuaucgc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gtucunbzy.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gkklipipd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gttrfcpno.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gtqmsijrc.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gboopqjif.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gvliivtfy.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gpbqefrdk.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gdajhaekv.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gcxxisxfe.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/geioeskfj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gttcefbfx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvmlhialt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gyykawjwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gikewqyla.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/giakszpoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/guxepzjwt.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gqtmpybfk.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gxssytkud.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gjxudnpmo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gkruhmwca.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/goawgmfif.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gptttjscq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/geezeslsf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gixzvyxeb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gddlvfyus.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkpcuzrmd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gzjzshlis.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gyoaoxxid.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gfwxlkjel.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gbunwsnfq.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gbftwkzcm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gecthdpum.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gitgpbwca.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/goncrvhye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxskhmnjp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gyvppfeiz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/ghqlqamqh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gxxkiwkjj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gdyiwczkf.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gtwmnmqzg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gnacxwlva.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gwziacvcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gyardqkqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gxetcziab.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gxzashtxz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gheyxccxl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbihquntc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/giimldzyn.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/govnbunmt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/grkxxhutc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/ghywwueir.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gctqbourq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ggpltzhyd.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gjefskvly.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/glywhtgzg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gghjimlms.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gtqryiqoh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxadjogqq.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/geirgldgk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpfegqnbd.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyxdyyivl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gkbtuwqeq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gimicqhsp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gkthzhuyl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gydbanggw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/ghhneuhee.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gwfzqvtpw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gpdwpumxf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtnungmoo.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gwqtkgbab.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gwhqabzdx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gbazrmmtq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gbxuysrvs.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqetczmgy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gxqnrxotp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gxokogedb.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gearykkyc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gdnvgbsxs.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gswehkufc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gjztcuglm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gajkblcfx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grajhsfnr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gblvozjtk.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gtlzhppem.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqigjihwh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gvimtlanj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gddddekod.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gkgggnjbj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxmlwtj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/ghikyapct.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gtuwhsetj.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxtztwksb.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gcetywkek.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gaexrdwmz.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/geqczixit.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/grvspqvoq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gaapnxxua.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gdnbymglk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gkxuucyln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gonjewlnp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gnypgcdqo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/geopbgvrp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gqpzawxav.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gdqtgojem.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzbrfdxgo.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/glfsnpsoe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gzuaizwtr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/ghzuciqyg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkanyqvpf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkefeuxyv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzsppnvqi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gjkydixsp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gifayctbo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbezljtic.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gjfjpxxux.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gldevxzar.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gbyngzaxs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gdljnqbvy.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gslwcuqdt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gcwvgtxxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gfomfewly.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/geqzudzha.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gsjkxgubh.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gltvzvjhi.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gjedrdcqh.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gdjeizhxy.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gahhwunku.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwwtgxjcl.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gssyeyiji.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gpezjcajs.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzzwpjcim.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gjbtweeaf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gcqgqbwyf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/ghaseaqhw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gofrpdhez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gusxamvfz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gkdhejper.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gwcoflhif.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gkipjkexb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrvkrzjy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/galtqcwar.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gnnhkjnbn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkuxtzcwd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gegxvxvrl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gnlntigrf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gxuehuyqu.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/grbbasmin.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsyqtifxq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gxxljvhpf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gbdsrlkik.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gprrojmzt.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/glkyqyurc.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gwlpvypgu.sHtML


<!-- 参考信息 -->