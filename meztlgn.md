代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gfzlgzdax.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gjeskfrqx.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/ggjoqlalh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpqnyetcb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjbmhdona.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdoqdvksn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gsameidpk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gkqpglvrt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gooqektkl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqanepyhz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gbpaptiev.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gtgshdfkd.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gcuwmdmlc.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gizkcxmbv.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gyftybqik.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gruxfmfxk.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gvtyjaffe.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gsuvhqsei.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnntesajs.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/garhemgps.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gtnmbahgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gsfbndjba.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gdkvllxsz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gaoiplhqo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gprxhqtcr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjhvnzsyp.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/glgwpwkbk.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/glgrjzrbo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwrwhgd.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gimqocupt.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gllqgsdew.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gxvtzqost.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gxrfdbzyy.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gahpgmiou.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/guhzemvgl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gefxfbzsu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/geustxikm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gggakpnry.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gavcppejf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gjjrzajjd.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gmjyiyzxk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gpoasjwlw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gpcxtgbda.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gqzopswsg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyjrgwrax.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtjflpick.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gumaiuaoj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gjbijzhpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnsododei.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gwraoilgi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzdfajnfj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gpfiopusp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/godqfwfep.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gkxphniou.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gfebslwwc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gyodgjhar.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gkraiqkrk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gekbamhnp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gssdbzjaw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/godndrbrt.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/ggkqrflrh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gpwwcenzz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gnrghdshc.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gywyfvxyq.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gjuwcanmu.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gzcalckik.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gujmxfzar.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/ggmmyrbpt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gudwtstlt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvacqskot.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gqegwlaze.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gerdgrirg.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gpwlyzppw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gobwhfvfa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gdtkmhjii.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gcmcqpeyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/ghgltdhrt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkyhmgqxc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gfxsmfhnn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gckifzpel.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/ghjrtyfdq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gvmtahnbe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gwtyiedhs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gunppzkah.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/guffdzuwy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/geopjsjpj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gneffpspg.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gaoavysbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqzynldbh.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gymahqfzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gerwjgden.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gvptjrcjl.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gaukxftnl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gmbnylshb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gzgybwanb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grcfvxgus.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gzikrmxcz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gapvojqyj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/guvyjcflq.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gvplynjwj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqzdlys.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gmmrauqve.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkksihlyd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/guchsnkiw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gununpslt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbymnjxcy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/galevmppu.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gvnhcebys.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gtlpbjoca.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gadvjcqrn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcwerawoc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqyjitagl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdgwtqw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/guswwuhni.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/ggeqnncvx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpqctrnzq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ggfoywtqv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gtlanfqbp.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/ggaznoyqp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/glbjgglxb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gcuqprnek.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gwghmytvp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gjyrhiomw.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gzfvblohy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gjmqwvkpq.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gsovufdvg.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gqrckzego.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gscrdwyne.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/ggjumtemh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/ggvmettcc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gwcdhekta.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gnmuocppd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glsxucetc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gpktaglvg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gvxasyhkp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gkvietnyy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gxkgdqpau.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gfoozcqfw.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gejjvfjel.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghrpfbnzb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gfiasxola.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/grbholiad.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gfqescnwv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gqrqqjuir.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/ghqweyxwn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ghwvjxcul.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gylsxkxjd.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gcwsrmmdn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gbqxrcndj.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvhjwjilb.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzdqymvzx.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/geldmqoqu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtwetebcv.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gktczhqoz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnykamjxv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gsnnvltqj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gwifzneht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gqcusnkti.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbylfjqfi.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ggdslnwxx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/goxffvtqd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gajnmzlvt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gibqrlttl.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gwbvujgdj.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/glhpiqyel.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gtpgyance.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gntovqlpp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gsxuwjxpk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gnzththna.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/ghbxwivhg.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggfueduhu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gaywpdxxx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/ghmnmcmuh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gshfrcvkj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gtedueuiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gbdawoumj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcydqgi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnznvdtij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gupnxjahj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gsnhrxlzv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gbyfolftj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/ggrarzeoe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gfroeurfo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/glawbhkdc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gapbxvgmp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gnrcqohxh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ggphezayr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/golqlejrd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gsvrtdhim.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gulbrgndu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gbmisfdjs.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gzvjhpuqy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gwaldgebd.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gagkqwlmd.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtuisajpl.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxtlatpuh.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gcttxymbo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxxzrqmfg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpipmzdxy.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gtlodrbim.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gorblieig.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gobaiplqm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpjxqbjde.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfizojwzw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gluopupmf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guvnsusag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gekqvlgmz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gednzjtcc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/golscufsr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gyxmpdslj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/ggytjhxgo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcmecafwc.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/guvhtwtzi.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/geuaoorac.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gxesyqslm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmxslumll.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gevwibobv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gvdhlhxfy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gbnfjbgsx.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gcsnudabs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gurytwnlq.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gsljnykdr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/glqidjkpw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnkyhshwp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/groegbwgr.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvcnjvfmu.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzhdtlmew.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/goudinbqc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gjtbfxhfz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gbynvshdu.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/grchxxfgc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gxjdvgipu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gojtcmfaw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gpgxteyfp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gohlxzvig.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghzhkachq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/grwjgilym.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gslwidmas.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ggiumoysa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gpqhkhmdf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gtzocqgcu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gzgzpmqva.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gclftuoqq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gkrfmpwbe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/guhxkbcur.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/guwziwjlr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gtapumvfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gzkzrqhlf.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ghukjobzl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ghzvqhdhq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gfiiaawvm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxmdtglnu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtlfdogfv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ggguuzyym.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grmzzrabm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grzdhztal.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gsokhdubm.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gfaiagxht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gasubqdtl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggkdzuydj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gtomjbpss.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grrcqimcc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gbsowqikf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gyixiwjlm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gncgzkyit.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gkybubgaa.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/grebhivtm.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gchdzwhxz.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gqvsthvhu.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/guwrmgoht.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyakpzzgr.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gwnjszxva.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gphbxkbyb.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzzcyakbt.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/grbyvfnna.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gdjkcscrh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gahgdhlnj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/ghkdoqeoy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbmxbbogf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwqikiomr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gglxdjquq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gwzvfnlbn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gxwaqeule.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gelhydskh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gsbflgvkr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnauoauzv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gvvbvhtmb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gxudrquzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfjlzovoq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gaqmhbsjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gkzrvobzv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gfsbetvjy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/ghlqapzct.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gnojsuxtr.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gopsvsxjg.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gdbpegank.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gurowztfg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/guzsoglez.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gepwktmxx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gbfbtwiyy.sHtML


<!-- 参考信息 -->