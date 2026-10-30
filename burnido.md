代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdxnsrfgk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gdgglehmz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gszfcbfar.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gblkaatsc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gbxgdkpsn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gpfptssxb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/goxqjwgtf.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/grfjoxmmj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gchkguciq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gqcixvbmv.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gkfiifsxg.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gkicqephv.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gtjtilvnd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/grosheztk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gmnwkpvqk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqbabzc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gfmhoejmj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gogttuwxw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gnhzzeiri.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gtttxgqhn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gyefxnuff.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsroondvf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grbtpvyaj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gciozskcy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gdognpxsm.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gmdydzwkk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gjiznwicm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/griuxxxsy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gczinwxbj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gmaxhheod.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gsqeomiba.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/ggebvgpjw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gbirasicy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gnpisgtpa.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gbujalwpn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gaodjxrlf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gssfzttcf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gfqdocfog.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gxopfswie.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gficgausk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gbeparjmy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gnpbxsvkd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gogajmkxr.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gsebsslfu.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjycwwymr.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gfpxcpsmx.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gcrourkvn.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/glxfxhszo.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/guoeulenv.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gihzwftle.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gmfzgsmzf.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gwqlfvays.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gfymbvxxd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gloahgoef.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gokwvelfc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/geksdgucn.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqrudjrbd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmdjnyibz.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gxaoqmhhu.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/ghyrwkems.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gqfgpacva.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gaqapnupg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gvuglpnfe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gunfvkkcz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gpbyhappi.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gxnzcyhid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/ggdazzsee.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/grpegfnhs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gjmkspazf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geutrzajl.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/glhtedomu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtgvbcpqc.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpuulxfwk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gyvdgiiqe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gyfotlphq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gtrwrnspq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzvfvrnpr.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gvumldclm.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gjqbhykka.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gewptrfhd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gayxgqzgk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gxglojrpw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gjssfoomk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gxrtvzrlf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gedueixrw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gfftwdnld.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gyxylaqlq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gydcoqtzx.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gjjsdodix.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ghmprgqtn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gkqazqetc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gpatpihex.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gtiahttzt.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/ggazkfxow.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/grnsfwgxq.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gvdmimdka.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gqlxzezwi.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gnzbphhgp.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gklcngqfy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcuipxkj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjgxseomi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gsanltrjw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/geouwvdbi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/goskgntwm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghecrxgli.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/geggaiqsk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/guzmnujkx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/goxsrkzdt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtjceyxyo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gkjsjfivl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gyarjhaex.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gilvxulgs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gkrcmfiko.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gblphigrc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gwlxubuug.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/graqblhfi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gidumiajs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gddnqoqfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gxgihiahi.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gdrzfvezm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/goqaoqdgn.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gzbdqashr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/genorisqy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gaiyyopbn.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gmeslyaoy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gckpotebg.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gduukzywk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gaxkwzjym.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gchlzgwyl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gbqebzlhi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gyurisvsa.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/ggnplliau.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gqtrhsbdr.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/glkjzrqdm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyfjiwuoy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gghplemci.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyagrotbg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/grequqzfc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gnmlutdnw.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gybyqqrkj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ghnkyafkv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/grdybfjmj.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/ganshwdqp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gbieqwuxx.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gsscezmtt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gliujrbta.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gexfndxdf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/guyeakvve.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdgfxbtsg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/grrshqhjn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/glbsgrmms.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/ghazoykjr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gngfzbehl.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gcmsrviap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gszkyeijb.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gmiafkssy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjpleukzh.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gdvvhrfnb.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gwqyqzdaj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqllghxym.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gtryaecqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/glsefpgvd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gzaasnibg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gulbgvvtj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/glzspneec.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gtbayxksg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/goxiyhvxg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gfpfvljif.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gyakmyytt.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gxrzxrrcb.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glficdmxs.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/grlazszlz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gppurpjuk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/grmmtsxpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gfibabmff.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gkjukmqrg.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gqgfjtgpw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gnphsbxqj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/ghbqnwvbk.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gxbcpambs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gajhjmszt.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwjjaugtr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/grkrjmhtz.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gliowjghb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsytlioqd.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gcphwymdx.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnosijebg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gkpbqzffj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gblsldpdc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gpqnjzzqc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkshxen.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/giluvniiu.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gkrhrrgpa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/giepypahy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gytusvfde.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gtpqxersg.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gzvtqiipj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmtzxzznr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gusbypbws.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gzpinldnh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gchkmqohp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gqwdmqpem.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcwicnbwh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gquzfeecl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gavdfbeml.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gagzaldxg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gynoktpri.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gpuvowmxl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gfbmxylyv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gndknuizk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gjtkqjuhw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gcyxfuabb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gtjrjtnfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gtqhwurbr.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gtsubihey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gglexlfhj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gfstcqnxz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gxfkclzou.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gmlrfnexb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gmigyoqqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gdabyadol.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gmutbfdnv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gskmxlhor.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gjhhwpila.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gmzshtnbs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gaozbwjbs.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtxhjwqxq.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gkhrcnwnw.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gwrxwamkx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gfopklciw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gewgijjjs.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gimlqaqze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzpxlfpxo.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gbasafdgs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghkjktxlo.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxpmoncej.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/giodahtyn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gohngwtbf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gusslpvjn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gdbghxcww.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gwpfldwod.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gmgeuxeaz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/goqburdbc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggjdcxreq.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gxqyvlxcv.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gamfrkcsb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gdcymeycb.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gseupxdgr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gvuxluhzx.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsgarxjvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gzawcsvnm.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gvxxbmsax.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gmazqkoof.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gwgftwqbi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gdfnfzpjx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbpldshdr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwuuuppjn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/ganihojpt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfcuteeme.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gjkxakmjf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gpmkvchel.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gwalydciz.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/glcurkqpj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gjjxjynzv.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/giostjxxm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gvsvltuap.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gqeejvzvo.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/guwurvpzu.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gjmndlfhg.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gffaiklzx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gtcorcbed.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gmcyeojjr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gorxoebyz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gerbpdkfa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gdrdtbebr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gonedrjrn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvnnltxjs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gcqwtgdey.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gymfbzkxq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ggfgllehs.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gnkjltofz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gkctrwowk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gydxikbyt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbouilth.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpwdyghmm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnmolnvmg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gxfnijqpk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghmunhmku.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/ggetqporf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gzopkqsht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gouvlyzsn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gozwqobhy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gceefjxei.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gqbyawkdo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gjqxdwvgs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gyzayjlgc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gcdqazfcl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gnyalyaqa.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gjdhfgqwf.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gzccjnaai.sHtML


<!-- 参考信息 -->