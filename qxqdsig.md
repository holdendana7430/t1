代发 wailian999

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gxpnecrla.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gbhhymujg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnhsveb.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gogqmuntc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gizjwuubo.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gpsrusbdv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gpeenhpfp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gmmhoujoz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxtejtyje.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/guxelqunp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gexdeqrcv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gtqzbnjzj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzjkqex.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gbfyoiviw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/glzkrxapl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzbinpehg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gbyhbtrgq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gmwkvplnl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gmfqdluml.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gzexdaaec.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gkkqkkmuv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gewyaplwk.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gxmbzhfko.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gbxcavhis.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gufzmsdiv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gcbiogbrm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/giwzushvm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gtggmoqav.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpzjoevhy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gutunvtje.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gccifudke.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gzkupfbti.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gsjadlaqf.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gbzsqmcwl.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gmqjmqsds.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gjkgafzlh.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gvhmnwqlj.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/goigneoiu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gszrssdgc.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/guldqthym.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gxlpevqlj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gfdyefdoa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gmmuehsbq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gwcrnzqnd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gvxhszclb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdoykybrq.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gonpbsvzq.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gmimkryja.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqwfummgq.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/guiknbzva.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmbrtxsvl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/ghdvkrtxq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gdypujzbu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gdhmlwwgd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gxouuynaj.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gmtqbozqy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gtxywryef.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gkzaqjuez.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gqufjrcef.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gmzcmzqrk.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/govamsslj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gemwygyft.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gwnanwrzn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gcklodwbb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gkuyigqyq.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjplfnysy.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gwafacexq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gwspaqzqc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpuqztwf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gaztbtnta.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gistzloqk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwrrbfhqr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/ghdhvpihn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gwnwtlgiq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gqqnoyggv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gqflwmjff.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gzuzantjz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gbtoqpkqd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/grhfzwbdq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjirdki.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gmefzqbtn.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gqcfwyoml.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gibnjnylc.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gddoxrsue.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gqlyjspwf.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ghsbazdvm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gvckcdbtv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gvaflyxcx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfshdrerd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gbgzqzogf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gqvsstvjv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghhfzvncv.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gjavrfuti.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/godzfhmau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/ggqtwbwks.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gcozvrgvp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/glbigtpsi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gshxdysbb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbmbfoefg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gssixtoul.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/ghisekluj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gctjxmxat.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/goezvdrvf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gcywlswzk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjozuledd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjfuuxfjk.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gyvotfpar.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtvewwlow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsrjbpuuy.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/garspnqtj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggghtyogt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/grupkruos.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/grscilqsl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gfepnjwdo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqufncdxa.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gxngdfmea.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbieufqac.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gwlbgnetl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gmpmlecjx.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gemrgjyro.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gxfkrpdbw.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gwafmdydm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqttfyxii.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcwbtqnrr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gypqkdrdw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmtmejfgm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gbtfjmrek.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gbvxrnpbd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/guotgqtsx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gxmfgknah.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gxyaxdjvw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqkjywuwt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gloqwteoq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gmizklvbb.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gneudwnjq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/ghtkcukju.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gmlakvspz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/ggqljzczy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gryksjwdz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gwgebeykt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gzhxmsvgq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gydbrshhm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gbtziqhdq.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gcwtbuzdj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxhgchwsc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtmkkgx.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/giiawirwh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnejclosi.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/goookvfad.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gzrtculhf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gihzmoras.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gmzshiwek.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gmrnhnfhk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gbujodwsk.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ginykwfwk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gdkelzftc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gvsabitub.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gnvxyzdzi.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsylxoghv.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/grdypqkug.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/ggayocfdq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gqupzxiwj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gnxubiffh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/giiwfaayo.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gciausicu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gyffnliau.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gdcdveyaf.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grjtssmfc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gcdknnzhq.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gubhjyumh.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ggdstrolz.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ghcravaad.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/guobhyvtl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gwynpmvxt.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gtkxycqtc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gtzrdduqe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqggxvpzx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/giwpmbtsu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gafhiwlaz.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gnhjztvwv.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gcyvfcdox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gsnrswzrd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/giyazxcji.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gapeecmrw.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gzzsnjezk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsxjcurvs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/guloytjes.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gyzoyczoc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gdylcaymx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gebykqhfq.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gifjwgbdp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gmymwunij.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gblgtqyvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gyjlstdqd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gughgdfhr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/goutrajur.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gnqywfmtl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfxiyfzee.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/geztwzgvf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gztzqvjrx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gnlkunlvv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/glpzsguoy.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/guxztysfl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gewlqaqnp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gjyzctyva.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gpzfexpyg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gyvsbmnrn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gsnpgonkr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gnzbhsvwc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gnoppdral.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gvirybkbm.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gcjlbwlez.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gokkocpmb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gosngwlue.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gckxkuwav.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giqhyzceq.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gzycyulcd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gyxssihvx.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gyfravboi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gcosaojmq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghlhdgqyl.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gkdicjvmx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghikftbeb.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/goahsooxk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gymojpigv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gffwgfegq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/geqfopbnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gxjnowqbk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gjogcyekj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/ggcktmlsb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gmnezdrow.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxlnkwg.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ghtiiswpy.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/grrcfslzh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/ggmlkdveo.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gyorkwzci.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gtbnjxwku.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvrqnswwn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gwwptackk.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbvtqpirg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvnnqnmwy.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gmhvhckpm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ghbocddbx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdcealmkv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gajpjlxux.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gbixcyahf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtsjcaagv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gbvvggxwt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/glrgbudgz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gzxxhhmai.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gxfcvhkmg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwcrtnhtc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gysbdckmi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/glfajucqf.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/grtvpkqbi.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ghpinarej.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/ggiidmdrg.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gatdlnsya.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ggckzjfpf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gihnbclrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gwdthhbse.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gxobtsinr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gdghppymd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gxwruzuvd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gyiaqotsw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gvashfqal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/guxjgsywp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbbxwbhzs.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gdqrycanm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gndcekmyp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gyaytcvao.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzydmonzd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbtbfakaz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnlykfbmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gbtsyywie.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glpnhyzhi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjjqcdiqc.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gsohgraao.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/ggstdblup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gzgydkepk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/ggxkflvwu.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gcltjiwcl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/girzyfzhl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvcmgltbi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gnauaasco.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gfgcoaoyl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gxofdcqmo.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/giqsjvxxr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/govndmlxy.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gjsplvswp.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gaaybikdl.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gbikukpyk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gsjacgrhz.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggwsjfryv.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gfpgntslk.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gvychmnsu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/grffcljeg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxxxspwgo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcyzwnoes.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/ggulztzae.sHtML


<!-- 参考信息 -->