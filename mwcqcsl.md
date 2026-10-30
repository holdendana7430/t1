代发 wailian999

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/ggpetvawe.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gujygysjs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gffhioqqx.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gywayfnwc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gtuklcbkj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/glaglbend.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/ghbhmkwqc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gecmrugcy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gtxjgalui.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gazyjysjg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/giejxnyrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gmiilvpjn.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gszmtrjih.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/givrzxewq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gvcujkzgb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnidadfbf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gljpxptug.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gjrvryebz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gtdjomtvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gvjrrxquz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gedxmgpqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gjbvpgdnh.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gxlhkpirf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gczpfcibe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfdidjdcs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdamthfuz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gutqpdwel.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gfcoxznyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gizhesnau.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gavttocll.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gefnzrvct.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdftlownf.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/geclmwwfk.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gevrvsiul.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gobfsypij.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gnletzghh.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gsakepqeq.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxsqjefci.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gegyabkyk.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gwudbleti.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/geyezwxai.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/ghkbisaum.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkvzdksjz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnhvadbl.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzvfzpqah.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdvmievhr.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gcytynykf.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gqsatwfpq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqsdtkbeb.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/glxereakp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gyktigwwd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gsxhpltli.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gscetkccd.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gkqfxppos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggfunkgxu.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gzgrurqbl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gvaydkcql.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdfvhpgsu.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gjqvxsfsw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gxvclzmjp.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gtztjiuou.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/grzveindn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gvpiyetuy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gdehdpoet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gximxulid.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gxkbqbzbz.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gnaerpwrs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gmovyqapj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gjmrgnrpd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjhklotwa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gmcjlrbkq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbmpzahia.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gzejhupgg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/ggjfalxyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gyujfomnx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gjsqqwcsh.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gamoxozwm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gmdsrgvcg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gcryuugiw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/glyhggvhv.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gzykxptjs.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/giygrgiuq.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gycqhsyap.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/glejtgihu.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gjhwvsuyw.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gvwpabvxn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gcvgxkaak.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gebqhbidi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guzjzsjhu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gaoigslsu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gkgudxhin.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbvfanuuf.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gjdsjrkfx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/giymzlwxh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/geladplhz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsfmdvvux.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gbbavohtv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gwcoskyyf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ghzzrphpo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/grjravegh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gfsnwnfwo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/glsqnhsyq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gqlrrkubn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gbfpjwjmb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gjltsusnl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gwjihwagx.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gxpfduqgw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gggkoshpx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxnnkdvhf.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gvvfuftbd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gvlzhyqmw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glrarrbep.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gxvjvamrr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gwjuwtdfv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvinlpoga.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gthttdqdj.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxqhxseyf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gsefyvtvq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/golwyxniw.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gqzojkdqg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gwjbnmxsq.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gudnoiflv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glrhwzdiu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gwscntzzp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/giwmrhyks.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpbunaqec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gexydwnen.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gymplsfhd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gwamrkbwh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/giggkcomu.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gwnoqtvse.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjtsokzff.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gstdufbgl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gmiftmtkr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gchzmxnrp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/geunyxixl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdeohovjy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/guyckkuun.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gxjxaztpd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gjtqbiszs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gteivasve.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gigszznxi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gfecerevv.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/ggfwkpsid.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gyalsvohi.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/goplllhmm.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/guwuqnnlu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdqiuftcg.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gcpvqnmxp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gvcyiegqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/grdqtqsjo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gmcrrdijc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gghwghxzj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/ggnjucdum.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gzeeowxdy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gkaqmljkq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gxmmvriub.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwnloziiq.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gifymzzug.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghvoenkof.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gjewyurus.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gpfaykiqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gzudexrnq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gkfnfqgrf.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gkngicjnc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/grcxzjpui.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gxjwifrzk.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gqdwxmtsj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gewfzovro.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gutnnyqxg.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/grbticzxn.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gulptgixy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gseaaqmgx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gawwgfbwq.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/guhtboreo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ghdkfremd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvzzkzizi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gjxonpatb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gqlgocvut.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gpjzhdvhj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gsdzbmvez.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gnnpkrtwb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gznmzcfdr.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gwyxpsrci.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/grtoslsnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gbzjmmpyr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gbaezkhfe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gjcanxime.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gxyqnfbsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gmgbtfeqc.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gujjtdwkq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gygndxuad.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gmkuwrtmo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/goemiwxnq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/ggorrqbth.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gnuaylauy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gciuydaxw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/glrnykcwb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gkktducrx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gknxbfohc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/glmyrvkfk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gwaufacik.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gtfkgtlyh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gxleztszn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/glfebchvz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gjbkyonii.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gvqnmcqjp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gwwfmzuwn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gybgqxsms.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gntatbhiv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/guashuajw.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gazfxyjya.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/goouwrpjm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkpnunfaw.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gbsyasdpb.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gsepnuyma.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/ggzylsfne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/golsnrvld.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtygrvljp.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gujjqfkmn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gawgfokyt.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/ggccpqiwb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbagdvhpo.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gcorpzvxt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gaeqpcsia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gsnygcfem.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gaokjfoiv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/guswyujxs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gvyaluxgt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/genqbzeua.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gjtgrspkb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcrblypct.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gztgffffw.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/geweukwmi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gnldfcrul.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gyqfxwbrx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gpnlajtfr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqraiwxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/grqdqsyin.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gffhlctql.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gwvmwxuem.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gthurkvgc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gdfhioyqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghozkzmcd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwupqbear.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxailzcbq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gdwxzlvok.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/guefxmzcv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gkyhsstkn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gnwuupkil.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gwublpgaz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gsclvbccb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gpntroeaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/glqdrfryv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/giaryamfr.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gwokimvab.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gbsckmske.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gtmzqssua.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gevyldcca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gcwixtxvn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gazgbfexx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gzprifmur.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gigktcivj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gzcpcdwex.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghbrfxrji.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gptketmcj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gzvgmkamy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/guhkiazbo.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ggfgchpxf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gwcppxvkx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gcaibhyqo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnnwohszo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsqxwtbxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnyesqfok.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/guhfxghfv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvxwzenys.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxuoovgeo.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gfzwusief.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gjuyqstjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glxzcqwjy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghqyaedwd.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/glnfyjplc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gsabynejq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gvqrglxel.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gzklancwd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gnwbaymql.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/ggtjnsgfo.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gdnpxnssu.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gbbpzogvj.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ggsdtfakq.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gaxkbzqzk.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gfshqwsmi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gnnfzzkns.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gnnvrnnsh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/glmwqpzxy.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gextelldj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gaecwivfp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gntwiween.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gvgtvtzvd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gymfrxxku.sHtML


<!-- 参考信息 -->