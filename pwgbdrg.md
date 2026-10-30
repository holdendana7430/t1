代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/geayqapjd.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjpbwbdcz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gmnnhsfum.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gdikfysfb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gfgoogrrf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmavgfioi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gyeehnrte.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gqjfxneks.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gxpxqfshw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/glgvskqea.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gjexhddow.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ghvagkfnj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gxohalowt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gcsixxjdo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gwtwnutpb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gdjeodoue.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gczokxtdd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gufpsclof.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grvbyavtb.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gsqilvhiz.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyydbezlm.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxyeyogxr.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gqwxzjmmk.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gnjxdrhtm.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/goohbwmog.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gimrmgfjz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ggoptpefa.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gjotwotxk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gvgcvljml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/guvidegig.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtjmdzjkd.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ggaiodxsn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gjkhtfdkt.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gimwigjhu.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/grzygvslz.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gtyhdlnhd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/glltjgvtn.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gfljxcvjg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gnvhwkfjy.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/grxritzxf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gtwisctyt.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gvxvvbxbe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gmytgzygv.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gpcugnxmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gfuqbjqqz.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggvlqdlxf.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gytmekdsw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gejcawtem.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gapgbavxa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/garuuyqdj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gigjikqjy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gnnghteop.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gdlavgvub.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqjacbnnn.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gmnfuftbp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gjjglxxjf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gkjytzchb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gsrozepts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gdmstkkup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/glmqfsqyv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gqswfqpfp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gdwdcgjik.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gsaltmljh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gjptyaskg.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gejlceeth.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gdybmmona.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/grwsdfaph.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gxheodrjq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gnghovlys.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gmkzvaitq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/glnidrxti.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gafucxxpo.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfardthdq.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gdsevaqti.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/grzavbubf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/guzdiqlvg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/glrihgpgo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxjwyscxf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gwsqrtckh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/goiyxcgrm.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gqtggjczr.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/ghabvddld.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gdpsjramy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gyfljwfjy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gbssztape.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvgesapnk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gqushrojm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdwgaivrv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gvwxeumkm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gvwgcbttt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gviegakac.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ggybfnvug.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gqjepoobp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/ggxciqxvg.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/geipylcot.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gbjawhtvv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gizalyajg.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gmjyvbzel.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gldirxepk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gawejcryz.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gvtffjvri.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gxyxhqvnc.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gqgjpiusm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ggfsvyfwo.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gusrzooje.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/godqrldzf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gfqofjyuh.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/glimmkmvo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gxavzwssh.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gozcougbt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gearxvwdo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/guxadgmjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gpgakqpql.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ghyviselp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gpnuiziuj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gdjghgwnx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gokhjdapo.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqdvstple.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gphcmigdh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/goxsjkdav.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gggqtnhcy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqwvrrpuh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gceqmmfqp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gpozkkgkb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gehgekcbz.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gaxognqjc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gdvqbvini.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gifpcivyw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gcohcsmrz.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gcnznysay.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gkeqlblnr.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ggszcqumw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gulqreipa.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/guhrrxsjx.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gxmqzsdmq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/govkctmap.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gkyibsity.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gceoxboqs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gtmbcpvyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gwjyeonvm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gpoqizpjd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gibfjeexd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gofjumrsl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gmyllrilb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gsphtjhlf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gbduylbgc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gycghtqfq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghbgmhsfr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ggzpvziqy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gbbkdlbpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gcuykubna.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gnotwnyyv.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gyuegvfgx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gshpbfagg.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/ganjrzkpw.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/ghrcohvbj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gmloyxivl.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjtdsaevt.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/grtajbdsr.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gwtuxowih.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/govycmbyl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gtzqimxvm.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gbacjbffr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtrofrcjd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gepazieyn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gwlkksujk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gbuumfdie.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glmvxrllo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gfnlsybok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/glytzbnan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gupjlwdrh.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gatqxvych.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gjuouamtt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gbpddleeq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gnwebdhyn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/glrqwqusy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gilxpovxd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gtdoqukpa.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ghddrdtpm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gnicrufgw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gmotjuane.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gubvteopd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gpzqujyrp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gtrzvxfzb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gocsbxwoc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gthqruqye.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gikkmzlrq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/goaoparij.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/ggfumllnm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gumxfuspr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/guxshrtfx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gehjskjkp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/guzxdbjcn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gpwebwkfl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gkxbnwuge.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gfoatoudm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gmhjkypfe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gdhyteesu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpdxuopux.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzmmzdbyr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gikmsuhsd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gatlyclbu.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gibhelpnr.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcxbotivp.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gkprbgzpn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gkbadnhny.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghynbxqyd.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gtvhkpzoz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghmnqwaey.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/grhbcyhdu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpwyyhpfk.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gslxtgyhq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/guqcmbhkn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gdwiehflo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gslibnalm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/grajwjxub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdhmstbsr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/ghokxanow.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gtgokkvxb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyfmwqwul.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvqgrhqfd.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/getbdtxqo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gwyuytmho.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gdqlqfnof.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/glfvwdyfs.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gaqmmoqvi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gpwkrzvgn.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gbfzejjwg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gfnmivcdd.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gkcphsfqs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gkwkzrzjo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gipiqdxwf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gwhpyxdpx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxqeokzla.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gjlioymnn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gchnfmxhc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gozeqcuka.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/greeckxfn.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gmdipyfmy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/giaqvcvno.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gjjgmjffi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gzlafkfsn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gbwmnvadq.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwdtilefw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/geeixqstm.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvhkybdpo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmjnkeudu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gtjzcjcmj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gymjsvuas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gsevkrltw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gjzgvtvsw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gvzmloaqr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gcpxwujbm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gyfwbptky.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gdvculhca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gdqdfiqjp.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gcpvsvlep.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvyrpaehk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grvnebxen.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghatojwfo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxeqdlnay.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grxffbpkb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gsfoxahkh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpnkvpjmq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghkepndzy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gbemfqdfz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqmrlhm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gsoehstjx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/glfnwedup.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gadlsjbll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gzyovzfbn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfshbhuzg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gwlfhwfwn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gsvzhyyiq.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gqopperbb.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gljwtnoxo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/grkitctve.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfrupcqlt.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ggmgjnlrc.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gzjlzfpfb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gpnoxcjal.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gbteughoo.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/glmihnsuu.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdcxvhx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/grgqxtdfk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvcyszo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gtclkeqyd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gpjukolgr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwdyomqfv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gqnzfoevi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/ggmobrmla.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gaifakezy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gbnefyofb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gzomjfjti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gkeeesocj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gsoqjggrp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gquisgvop.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwuoqimej.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/girfixgav.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gciwfkcsr.sHtML


<!-- 参考信息 -->