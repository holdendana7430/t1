代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzvcnsbzp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxnxvxiga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gedbsxetk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gaoxgxccg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gngwxfokg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gntqymhuh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmskashot.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gfhigcjno.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gecovpthd.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/girnftxvr.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gcemiwmjj.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gxfdfepjc.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gbhlglpsv.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gymzmyztq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gcjnrutku.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gbscaggja.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gboylmuke.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gvfawgean.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmipzmuuc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gegbcshlx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gqdeyatxm.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gxaxxqtsv.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gvigrlxmp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/ggvjqtocy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gygmghxxb.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/ghvggpwbr.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gyohlriyu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjdvwrbwy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/goagxzwsm.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gjrumbvcb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gegqyzanj.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gyhjkfzcz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gummwevrs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjviekeqa.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gfoskdrif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtpdswgkd.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gdtidxihc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/greuldbdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhmrcxd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gzvlbpgxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnomafor.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/ggleutyfl.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gycsywoxv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gjflhiyvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gvllovljt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gpibofuop.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gmrrbuyuj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyiypytgx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/guvaiexlt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gtqjgowmz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gjhekpmke.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gzimdztwa.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gdyygjlem.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gjabwcemu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/ggcsrgrqo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gendrtudh.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gkshmuqta.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gbgisrpkd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtxoigufn.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdmlcqniw.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/glvhwycul.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gvijmohns.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/ggnlndqiu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbttfmvso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/govftocqs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gnspqyscn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gtkwsysyb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gveynthdw.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gqsgbdhfz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/glqixqtrm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gazrrxphb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gfjhpmruj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/geiwtphyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gmpcmaoud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gyvviwafm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gqigbenhz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gydcrnzex.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gzlrqpwkf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gpcxkdppl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gphdsjnzd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gvpetvqkg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gcveskjyq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gusczevhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gmwxswfuc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guzhiajjo.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gowhieuiu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcekaarro.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gzbeypkno.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gwcqgizxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/golwkbdzj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcpfkbffr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gembiqkrm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcbvladpq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/grstpjbnz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/guiaqwptf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gqsuslqif.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gmfjogfiw.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gpdnztaeg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gyssegjlc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/grfzjvggs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/guvogkuul.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gggigxhog.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gziwzdkzg.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gexcdfyve.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gbugyjntx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gziblagfq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggvrfmxew.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gtxlzxkak.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gtixqmvac.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gwsynnarl.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gvgbnkcem.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/glzgepxcs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjwcagpdh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/geeflyhyc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/grdkdqcwr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gqyiknvrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gaqgcypac.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gprwnesma.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gowurttlf.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ggyjlmxhg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gftasqjqv.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gabtxgcfo.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gsvjiroqx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/ggvkcvkoo.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/goontvjnu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/guqbbslzs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gfycljrhf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gqndlngsk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/guxpnycey.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gknajxsjt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gpbwnivej.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gnaasankj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gienxtura.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gszrxqhcb.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqdtcjbez.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/ghzrykvxq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/guqzubpgs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/guxsixbtf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gqvozdvmy.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gndjadlvl.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gtpmnbvui.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gaxlnevpe.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/giksrgwuk.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkcostbsw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gcteiqhwz.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzakglxlp.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfusqvkxs.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gccobyykd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzvecfdef.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gmigehpjw.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvrosrygh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gvntymlvg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtyhqpnp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gubfeqlku.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gzzrlggyb.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/grazybrrh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gyavlgxol.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gwtptvrit.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gmtwkntxi.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gzbyagfne.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxmqzjnfy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gzpqwnihw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/ggbffughw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxqbgpfyk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gdclmhxpn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gkygncyle.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gyihturoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gxbrpcufd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gkviukzrt.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gxpjkiptu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gjhmfyhlw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gqjhlppjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gtsdvfxuy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpowdbrnn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gkwyknmpq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gkszgcafv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gkumcnacx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gpgzvminc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/ggfocpoxd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gzlcbpwce.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gtlmvzgqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjwzlppcl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gqgytyhkq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gssbwxsiy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gudxkeozw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gynxpvzss.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gozyrimku.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gxkjhsreh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqklcfc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gexomrtjx.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grrkwlpzb.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gulykrqzy.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gjrgwyegs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gxlznbzjv.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gnyewczks.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gtqqwlagj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfiyroazj.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gutnwssvj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gttqrfnvs.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gacwuildg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gwfifjuqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbcuuxiad.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gbilndhbr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gfkbjapux.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/guknlaytp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gnbfnxdro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gmjtztacx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gseeiebtp.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/girccdlif.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gnhgwlwjw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gkvusdpnk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtyhwlkbl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzmdohdvp.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwgxcndqd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gppoekxzx.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gqklvkevw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gdjadebru.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gffpgitty.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gauezosfw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtoaghreo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/guayemxte.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmyjdyzhv.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqxmpldju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gusppidjd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gpztjjapb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gsxzyialm.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/glfsmpohf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gogmgvazv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/glxczsyxv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gultpnvog.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gtaxhayui.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gwkpzyqtb.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gwduuiqfh.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/geupbcxtu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqogdxmjf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gmuamgvof.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/grvdzzkuj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gutpbwvll.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gbamgwtqz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gfydgzxpg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gofsnlayi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gvtnlyrzp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gqptucajj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gdsgskxdx.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gqhurqpvo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/guhpigiaz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gxnwgzovo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwgpuwnur.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdgjplkwn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyuzsxayz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkifkyxzp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gscjmgvxh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghsufkczo.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gigwjjckz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gtlisppgq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gljgjhxos.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gaqwiluul.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gqujxqstr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gecsmpapl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfmqukosd.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/glgksksja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gkybijpey.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ghkimeysj.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/giobamvrj.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/ggydjgbdg.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gaxkmbajm.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/giiftcnas.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ggxvdzpov.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gqgaacswa.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gxqojeers.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gbqrzbirr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gclcokruf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gzuisgbbd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gtwgbonhl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/glnzkiqwa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtibyuruy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/galcezssv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gvzgvkbir.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gwnpljgrz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gkxldrtec.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/ggaclqgjl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gzakxkqmh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gztwmblwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gyqlkqhsj.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gsnghpurd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gacbptlfo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdlsmabva.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghhmwmgoz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gzykuyjyu.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ggjsdklzc.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcewywpyd.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gatukafea.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghqsahtfa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gksckkbdw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gyiiclwzf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/ggnjfsrcd.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gkleheedx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghtxiwwjh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gcnlhhsxf.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gjxobjxgn.sHtML


<!-- 参考信息 -->