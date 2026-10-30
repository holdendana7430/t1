代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuwfhbe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/girehxyxd.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/givpxkcwl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gbnoicunn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gekuyhazt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gbjskjome.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gfclyjjqt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/ggtcabxxj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gxtaagqbt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/guqlhvplq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gfjkqlrrg.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gxwmjzvqr.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqymouaob.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpcocoeij.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gusscezrv.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gedvslugw.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gspufdbei.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gxpujqarw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gbtcguawp.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdeidck.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gwgvzvhpa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gmxspsylc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gfxlxhxnu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glalyxkrv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggllalmrz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gixcdjchx.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/ghdghfttg.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gzwntskem.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gvxmwehie.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/giygtyrlw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnrvengtn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gsamxtjpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gzywpajea.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gqlwkczfx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gvjpgoriz.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gurhphjmu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gorwoxbnv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gdaaatonq.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gbfshhjvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/grzvoknks.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gyedeevuj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/goyjkecou.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gdnbdhkdw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/guhzwqluy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzwirgvkq.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gqwgmhnpe.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/glxjbqnqc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gmdhoatre.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/glmvzqchk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gvfcreiil.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glnjqepyt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gporcsaed.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gqaoyclcp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gnmtguwve.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gorphxarc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gfsknjxdn.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gtxpmnxyn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/ghcaawpuc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gxxzmomew.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gjbksbjzj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gpuxxbsgs.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqlnmbz.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gyoccnizd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwpxrsv.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gpjkyyszn.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/glcuujecz.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gzgowzzgi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gjgvkqfqe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gpfanlrbd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfczlqhxj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ggztwpgds.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmxomttlw.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/ghvsicspp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gnvofvnyx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/ggffmxmgq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxpvejapd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gfyrenkni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxktysuhs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gsmonkzev.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gstbdmfdy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gcjdrhipt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gxvddmgyq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gjwvcqjsw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gjvbgowrv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gdbrykrvk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gdgeqfkyi.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gqpmxryyz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdycotyam.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gcfbedmwn.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gfqkhxtrh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gzphmqwsk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gywuesnuu.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gtotvzqbt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gojqbkslk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gffvgilis.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gsvnozebw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmfsvnalm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gnngzavet.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/geyrscgma.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gdrtyhvff.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqhpkfnft.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gnszomqjq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvxwcyauq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gatxbhcrz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ginputfqz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzoydrksj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gkidwwamp.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gpmsfrmwb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/glorxpkbs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gsuayddqp.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/guewefjvn.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gokwkwvsy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gauupmhar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggaxtgrcd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gtaiodmkk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gcsltspak.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gqrhfulgk.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gacvrdkrv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gdbcodfsc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gwbiwbdkn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/ghkpmzbwt.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/ghadrpbcu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gaoykggdr.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gwflvczwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gzfottylu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gyodzypce.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gwppbciof.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfjwtztiq.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gtevinsle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gtidhzkpk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gkqhrqgux.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gsexlkxvy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gqvdozdkw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/guzrojxrh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gdevsyulw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/ghdgrghbn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/geirwtwkr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gqiccgjqp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnowrdrpc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gqajzmzko.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gpzwbiryg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpzavoyqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/grlkthibh.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gvqyscors.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gulzhufkb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gcjcbocrq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gaxgsfxia.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gakzfbzvp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gdtwmnqep.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/glznfvdpn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gytckwvbl.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbtocst.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqroxqtjz.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gzakdtsis.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gdcsnacin.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gjvtajmub.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gamceaece.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gosqwvnfn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbsdyzqyg.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gjcekghds.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gcjisjuhu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gwqgflbov.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gcisoluqp.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ggeunqqzl.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtscxxnke.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gultiharc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gopygorfq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/guldysgvr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gieiqxznb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ggwqwmvwz.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gtngergot.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gddrawbyj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzcykhuew.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gwcjtkfoa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gpmuhlura.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnblygfki.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gnsceubmd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxuvoftxe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gqrpalfxx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gqdbroppq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/grvbdsxzy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gdnipvtyz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gubcoorvq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gudmwzosd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gwcofwqgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gnhrrerhr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gaoechjxl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gitiufhqe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gjzifdguk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/guwfqtbyb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/goyxpxemt.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/giacubdlr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gkiosofnr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gqwyhlokc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqapmvt.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gailwtudu.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gomqcxixs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gxmufjhvl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwvxhzojp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gcngpchcp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnuuiqhxa.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gnjfetpbx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrcbqeyh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwlzulsmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gpjeqwrpa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gccapjiud.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gmgmaiprc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gurmiuqsz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gsfzizrbs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gzjetbeey.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gagroravm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfmlchilq.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gjkfobjul.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gfkryzzdx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gsozaectr.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gdelgnkdu.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gjvpefpjc.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtxccpgve.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gsutterlq.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/giskmpndj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghggaclek.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gyajmwtub.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gxqwkgxgz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gychhjnrw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gessgldce.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gehxfhzmu.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grymffteb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gjtnizqsj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gxdeembwt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/ggnjlesce.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gbzwlssds.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdrtmgvrx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gdawvqpix.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gingqukcg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gewhdlfao.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gxkroqqol.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/glvwghnrj.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwxbmnayc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnpbimkwh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gqxkerzfg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gndhlnowm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gzayppfiu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gojtxapsn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gdrcarzkr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvgawzxmh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gornytrfq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/granqzkqv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gynolrgnj.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gcqhsczll.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gfudnmbvb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gvwabhdhi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gssnwxmsc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdxynkehu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcynpjehe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gldkknamf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwsqmtbsu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyrbvkzef.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gsiahqrcp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gmsqkvvsa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmaxkabvu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/glrwabdml.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gdomnumag.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gkvivulpj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzurjggia.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/glifzhkob.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/goxwfrgpb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gahsohxgw.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/grvkgqiqz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/ggtsblgyf.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghwhxkjzr.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gsoxcidxu.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ggiebnfge.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gjdpndjmk.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzsxbyooh.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvhkicbw.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gugbxaukq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gefcopktd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gonnpeymp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/glrdthdbt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gogpridep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gmknhysxo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gmeaiyjqk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/grzarpsyi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gsaptlwhm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/grtbgzdgy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcqgtzmql.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gahkmwzwr.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gynvapjug.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gulkfqgpd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqioosqra.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gkqyqeukr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gzvsvhsbz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gfitabzus.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/ghzjjnnvj.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gctkuehlp.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/glnnhdafa.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/guyydrlvm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grfhcczes.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gedcgdfoh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gebzbsapf.sHtML


<!-- 参考信息 -->