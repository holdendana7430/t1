代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcxzbivwn.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gluvuxshg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/ggepkomhb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gqycutaia.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwmrccfql.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/grczzzgga.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ggyfngxsh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gdihqxtpu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gwzfwlpcj.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gmycjkajw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gdanydhxe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gihvasstb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gvckskmyj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gkytsxztn.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gticxwheg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/goyaxnypf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gtxnmllfd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdeknynep.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gxuurmbqe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/glefticnh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gmqvofclc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/guhczipdz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gntgewaxf.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gchhksqvk.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/grcubxwiu.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggzqqymuj.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gnhtksyoy.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gqonxghtd.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gjurxkbld.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfeykvbcb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gycwnauus.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gsuhomkph.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gmgexrxaf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gmppgsdkv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gtjeqfxbc.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzvmmkrka.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gcbkzastt.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gswflftju.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gmfixdeou.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gqxrwfqcr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gpwqxnrxc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/ggjxwmxmy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gpwwtzgjw.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gajyftjkl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gfofekovp.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gtxjdoexj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gleeoezkj.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/grdvafunx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/ghvzoieog.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/govjbskrd.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gamwwmelb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gjqpsspbv.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkjviprng.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/guervthda.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gulhikune.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gwwwnqjoq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giudsblfu.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gclpmypjv.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gtgjyxprz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gxoysvjip.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gyuyopvjd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkkjuatle.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gnpddgmtu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gkgorceqf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwrxtav.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/grofxjstl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gtqzcjttv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/glwabkzum.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gbeugbyvd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gtcijwiuh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/ghnbrhmok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gdgltsmut.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gbilopgof.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/glkiadxay.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/geilqxbld.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gmkufllif.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gydvpitdi.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gcurimvam.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gwtndeyih.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gljoiedze.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gqdguelak.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvbltckbg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gxvrzxbfn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtpnvgjix.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gkraihjve.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/geiqnoyvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gnnxxfmbk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gbmxtrrqb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfuuqdxtc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gogbkmocc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/geshrgyym.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gbfhyqaqa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gpsjcazlz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gaovporba.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gaskwjcdv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gdccooywf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/guhdwhmkl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggdfcjezd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnvhvtkmi.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/grtonievt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqtvngwqy.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gumefprkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjentbtyu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gfwlyvqsn.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gnhuvgtpu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gujadowap.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gahakxnlr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjkpryffg.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gsawifzfd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gbilrjaia.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gklpfevmq.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/ggktuxluz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gauywwqbm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gacqpmugy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gpcxnblqi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gzpnlcfba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnlkmgsqe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gqxmdttos.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gwbazducc.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/guxbysxgf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gewsqevps.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gduckaymp.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gmfjtwsge.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/grtfhqadf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/geoipdjas.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/geykipizv.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcntshdu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gqmhyjmit.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/glpfrzyav.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gnhyaxtxm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gfsqzpyjr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gmlpjuvki.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gyggfbveo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gwepeypdc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/glubaujzq.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gzowakwkk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzdsdbtut.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/glzsppsfz.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gjgknwtnk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsfgbzqvj.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gxhatatub.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gkdqqhqic.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gwoolimpb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gpstcwkdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ghurfrnaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gndmlmgxi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gqftxadww.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gebyityfi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/grrvtudzq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gyyvrkbmy.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gspjmzscj.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkwavqtoj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gqczrjnqa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gdwzorkkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/ggxeyqyvv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gnquvcqmx.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/ggmrqlyly.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gqieehuwi.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gnjrosocj.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/glyoqcejr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gmyiwcyip.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqavsvxls.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gfpdqdpeg.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/ghumkjvzt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghfahdvty.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gllkgsrrx.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gndxpibus.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gmagjxrud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gebtkfraj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gnhqwvjri.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gbvhqtgjl.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gtpdvshlq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkreloxdn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gpxzusyhh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/ghdudqoew.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gaereyfre.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gtmoskiip.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsigjanku.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/glajgmcwq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtexbrjjn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjmcktlni.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gfviswsle.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gvdjinllg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/ghxctkhgu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gydtbziyj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gordwakvl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gkllpljpq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/glfzouflf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gcojeaebm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gppkhtfxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gkqkcsixq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/goqdgylab.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gxqnqphsu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gcktlayau.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gdmunxtbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gkixxwapv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gxklfotiu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gmzhloqgm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gizosxdkj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmzvlsxaq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gkbzmbtgc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gzbbyuiei.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gceawghoa.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gnwzvmoum.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/grericwpd.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/guegumlqm.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/geogmsiej.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghllqhfps.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gvzjgzckz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gybtdjzbv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gfimtlzew.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/grrixikxp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gprudcxsq.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gjszhysnx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gblfqgcwa.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gavnyqgif.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gvsqkwktv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gyppcwndg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjmqtts.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjabfmefs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gwaqzwbdj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gpqvqpbtl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gfiojmcua.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjuitnsck.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gyurusrkz.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gznwbmyzo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjqstrobz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghxidwdbb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghfkqiidd.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gppbiwpke.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsyarjiph.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsrpjyukb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gsvqdzbea.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gymgtekyj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/ghmghvdoh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnkxctutd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/guvznyrhd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnagacryg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghplwwsvf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gcojmsvop.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gxnsiisrd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gnfneykyl.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gtirppndj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gyohhxqht.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/grslfnbvy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gohkjdwbn.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gjmayyqiw.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gnsxszwug.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/galkdbuge.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gukyclymx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gwujkssri.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gtapajyqa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gsqliubpf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gdymlapdp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gnsixxirs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/ghqwifzdn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gklodirsu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gvpmelxby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/grxagnafi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gqpxcbgzt.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gzajcftpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gendguowu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gvktacrjz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbnkvsrbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwpdyxpjc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjvnprcpd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ggresawaf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gztvirlnd.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcqhnyxzb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gepvalqyy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gpdlkqtrf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqryuirzy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gfustcyou.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gdieqsbrq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/ggoanrqry.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gkklaehas.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/ganyuapwn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gibfqlluu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gficstrab.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gcjqkhdfi.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gxqphrktr.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gvndlytko.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjskzcgdi.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gullalcbs.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gexqtcfgm.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/geguzxmns.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gogxuoimr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gvebgbgzs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhdaohuz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/geyxsoqbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxqnibkr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gqddpcpuw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gjsuoeokn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gfysocuob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/glfsygirb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gvyzsmgvv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gvxkkjsbo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvbdklvrs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gpcohavud.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqloscgmo.sHtML


<!-- 参考信息 -->