代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gtqsarotn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqzherlef.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ggoaqpajf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gewufbaim.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxaxqah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gzdaobirv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ghykpqtmk.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsrlrcexb.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gggeopuoy.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbezqjtlc.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gajmbdlpt.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gezdyzxwn.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gwcaewuwa.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/grmnyjguj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gdhircoac.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gcwckxnfq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ggratfdzn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gvzbasunm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gtgsqpthn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdhjuyyqd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gysfdkffj.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gvucvkfwq.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gdurzylcx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gjnetorxv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gphxfjxav.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gfetveiuu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gmbgbtvkj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gptynywgh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/glxvwrhed.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gknrkwlpj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gwbdydedl.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gjluhzuuh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gqdfsurdu.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/giypopvct.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gplladrfq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/goeypyvoe.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/grgvbdfhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/grtokjxjd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gggbaonle.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/glgxvlnls.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggdigriiu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gflswcbuc.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gorfatomp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gjguyrgpe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gxfwolcep.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/guahavsly.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gbahuxkbl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gmryjuvwi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gsjpxfmbv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/giewpbqkw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/glmrtcyyf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/glplcdozz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gwfavaosd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gwgnbucqz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gyuibrmez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqtqblj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gthsvxjrc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/glxvfubbw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbuhwgllb.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gurrdlfoh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gygijrbbi.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gkcxeldcf.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gtlbhxyrc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbmqgtsfb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gwparexid.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gtahgkpzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gzprypwsl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glassrwia.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gnlixiwas.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gzlcqjclk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gjvucdjwm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/guaqbtxpd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gselakdeg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gsrbjkhta.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkppjosdc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gpwmdxghf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gutsytyuh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/grkfasnno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjzamzaby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/ghsbvpnbl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gjsbkxmtu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gawqeilkz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gwmbzcego.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwoiytmsw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gfwfpsliu.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gusxfdymd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gagktmvvp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gyvglpjnt.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/grwvakvbb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjgqvuheg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfcpvucgb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwrwggrzv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gojpeqfvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gbyhgkzeo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gxkdyskxc.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gxxogrrme.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcgytthdv.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gnyjwisaa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbsgrftkm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcjdydglx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxerbtrlu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gisnlccev.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gqpnbydan.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gyyjbkinw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gmlpsmuxs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gyfzhjdmu.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gqnacwoda.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/giymnspzf.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gyupgvykr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gbvvepedk.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/glztegwsc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/giaixogwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gdvausppe.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gzgwshlrp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gzdparhac.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gtqkmoduv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/ggukjexuj.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gymynysaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gkcgjuwic.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gstzqbebv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkzgxyjpl.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gbgpowzus.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/giryhjgck.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gqsbqhzav.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gfpzwpaaa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gmdkfcxsb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gvhdzerve.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gwamphurn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gdlsxmswm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gocuudtku.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gkyhecndy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gzoxoulxe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gpwnewvnr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gcigbpnpw.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggemjlvuv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gnopnwbuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcypdnlcv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gfmoxhjco.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gpisgdxgb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gjrfzrtog.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gfckusuzb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gdskexvfz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gdymysygv.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/giebywjct.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gfowksyfe.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gwfkyfihu.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/glbxabunm.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gangighjl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gubiuznpb.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/guyeoprfx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/germfjhtb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gyyhelfuk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkjnzbexl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/grrxsptcq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gfwuowwph.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gzxmbeqct.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gtqrggljq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gjhgwklah.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/ggsqhvwlf.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gvvuexaqb.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gwfebnfvn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gkqflebzj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkpiqzuaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdxqmjilo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gsfvfvilv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/ggcgtlfvo.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gshqtauka.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gymtcgovv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gesvpuort.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gqtasnynw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gldjxkyqu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggfcmbikf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gnksunsrx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfwjnxblv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gsygigviq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gwsvkmpqc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gralsnbwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gzzwmtiat.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gpmmhmdmd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gcbtnqeck.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gembaycrv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gexhswaiz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/ghstajqze.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gcukcxnrf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gtmcenlnv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gdlejtnxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/guwzephuw.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gvuanewte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/grasggmhb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gqssqnwmi.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grwjwegto.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghctvwesk.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gepeehbqn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gbijgjtjw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gbhpmcnga.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gzhepjles.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyuryiwbc.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gabzuwrka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glsynktng.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gvhssbygh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gdigjdolg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gievogzmg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gmjbfkzts.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ghxfvvtru.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gxiocsdyb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/glfnbrmcp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gkegyfwfn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gldzclutw.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gbagdixsn.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gwiorjuky.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gbgiulepc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gsxxqvovn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzsevqoq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqvfofgfs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gocuhifhr.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/glicstbsk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gsleirlri.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjlhrvclv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gnrnnjair.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gbcyohupw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvmmjvjqv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcsmxswis.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdfyijfqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gbldecgmz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gsuctoodc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gwpxsagft.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gkdhimqtz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gugzsqqzo.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/glpsyinor.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoagdqqw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gfwdmvyfq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gfzymctka.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gdoocylas.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqnyhpgeh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gdryjbcac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gfuzbshwk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gwbfihovx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gfijvbpnm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gjplkwybq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gqhlnwvzk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/glviqqtnh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/grpckinbh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gacpycfdk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsblhjgla.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gwizscwoi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ghlgqospx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gbsbjqmku.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glrppyatu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqwkeafoq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnzreedyy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gmssnwejm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzqcpcqtq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkhynzphc.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gviqiathw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gzkkqgvtm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gyjhcqncd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gdbiuuati.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnqkmvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/ghmamddjk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gtqstimdn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gedpoaakh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gkilgaojl.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbugwki.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gcihkzwfh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gtexfqeok.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gvmwutbxc.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gabjqgxez.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gywdirhwq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gglamyoqy.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gsznsdcpe.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gmqzksdnp.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/glozkkdnc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gtrltpmcg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gilscnvbg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkdjbpbwd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gwrlrrbtv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gvputvzbi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gtlkchzsc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/ghqzqmtui.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gmxwisisi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gwqxmcaud.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gaohtzsmb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/grbsinvdo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gqyfnwtuq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvycwmhly.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gqfsgfvuc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbfkqgife.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxkqyysqb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/goqhyfftn.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzltkppby.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gstqkttec.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxyskqswj.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmihqvjfp.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdbhvspnt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gyvgtzlmx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gfhjabnst.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxwbvgkrv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ghiyfquzj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/grhvohcnr.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gsfyftgph.sHtML


<!-- 参考信息 -->