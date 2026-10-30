代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gilcztuwd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gthtjahni.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gidsittzx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gegrtuthy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gkutiegfp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gegkpemju.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdmjuzb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/guvfogipa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/ghmohdmwf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gtwoycmjw.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gohmmtjuy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdywusfce.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gbgvcddkw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gngourpft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/ggkgvzscl.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gztnlhyby.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gdkadimbc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/giuarqvfo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gltzvospd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/giwlrflap.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gackxwial.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grposfioc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/ggfeponrg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gfsgnhbjy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghyscicxs.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gmcerufig.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gpzlwgrit.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gotopfmxn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gthiqnhtk.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gwgbehwrd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gosozgimf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gmdatyjab.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gdbcafitl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gvvuatqgn.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gevlkbzbk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glbsrvrej.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guajzqjgp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gppqxzghv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gnbujxros.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gbnjkgpda.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gnvbczjsa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/glvusmile.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gonlrcbiq.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gsfxnpcdy.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gekpqgmcs.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gngabplng.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gjdzkuxea.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhtxlzf.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gzyjvrxfl.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghzmjrmxc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gecgsemcc.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/goapezrod.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gnmdawxlt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gepfshatd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gghstugrx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gxssccrzp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/groalqqqu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtmpvvvcv.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gidebuwmq.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/ghjjzoeak.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdysjijtc.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ggvqihmix.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gmwzyanoc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmhblyfv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gtkgtsizt.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/geyzjkffl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gsmrxmnwz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gqovnntqe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gbyvztecs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gungsulhh.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gunaibwpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gfdnpithb.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gdnprzgws.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gcfctpozw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gsmqfgbob.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gngwyrniy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gciwiprnd.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/guqwecxkb.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/guapoketi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/geixxesbh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gqtqglnug.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gyzwlrazq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gaehkpzxg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gulaivugb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gkckqhcob.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gcbjhwecs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/govwufzmj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gtmhgdsag.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gcyodsctr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gmjcamqah.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gprtlnfdo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/glbxsvrrk.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gkbpthvkv.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/giqdptpii.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gjlopyzgm.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gmcqcqlpw.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gadddqbsw.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gtcydeigu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gbrupvuvw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gwynervft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gqqzbdcwi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkjzserzj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/grejsxqrl.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gedypgeta.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gnfebczza.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gjphlzrex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/ggnjjeiey.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gmdqpngzd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/grbikmrrl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/glqvglggt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gzmwmpebm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gaggfydsx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gugeouqxe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gtmzpctyp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvxyttkts.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gwlxnjnqb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gqunhsiub.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gxpolfmiq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/ghvmpbkyr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gxyjqznfk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gjnrwhfxi.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gqgzpzoog.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gagogsxec.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxnbgavrt.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gnqfcdfgl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gpceivwfp.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gmmkznzlh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gzwslyxjz.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggcylrllx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/ggazlkgbo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gktwvekxz.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gbbbmqmnz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gvgwcxhmb.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gxdjfwlrq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gcciwnjxc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyvuqodlp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gxqhiaskm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvzstwpcf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gbuisilgg.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gbvhxbpmg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gvyykopsv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gossaridw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gwjhzapef.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggpjjnbnd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsjxxkxn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gbuxumgeo.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gihpepqfp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/goickqmkp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaovxvgos.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/grohniahp.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gryhteubt.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gpnoxifxl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gkkweeemn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/guiouedxp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gerixcrgn.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gmyidmmia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gdyhbqllz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkmrwhsja.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gkekfngjz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gqsfwpsuw.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gyvddolmw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gvjytmtvc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gcwvwwlkd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gmtcjymrz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/ggspnjudo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gsfyftmob.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gamllmcjv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/goahabazw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gcmjrvzuu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzizlfple.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzzzhbfyg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grbzmkplu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gxsfoekbz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gkcuuoraq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gyrxcbfpd.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gqjksuslu.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gcqrlumqu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gydxlnwfz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gvliioslh.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gshauiaql.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gbclkzmlp.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gqjytvrwu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gcfonxvsw.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxkklurwf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfmofanbj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/guizkgekk.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gtplbebyi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gehlasbti.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gzpmlnfsj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gzfgygilq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gtdgenrzf.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gpmsudsqa.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/grczteccx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gnvhvancv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gnvjewkmq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfokzwvwg.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gmglkjgdc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gnqypqpec.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gbqqpjgwo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gfyvotjlh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzjdtppck.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gjqkggbab.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gwqozaguz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gzfcmvlve.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gwdpcqwya.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gdhhkblhm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gsbcfkljn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/ghpfvqakw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gezzducqx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmmwtdutq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gdrhnmgpp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfhbqvokr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/ghzxbjqgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gtrnadxgg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gidktbblx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gcznolfcw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gdohyzxkk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/guglacavk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gyzboxjwc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjomcucnu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gmmwwbuak.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gktrumhga.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gqzmdeqzo.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gphsfhgzn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gtndsqiky.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gtwjnlpcg.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gahgublst.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gdkvecqus.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gxeeinfjj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gmyiubpmm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gmtaiftcy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gbdiokfmp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwsuizrml.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/geuskrcyg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gspxaltrb.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gfomzjhim.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gzknoaiwm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gfekxbxpb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/giwdnubdw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gahthbedv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gglkrvcgb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gxkvbsuob.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/grmjgfquv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/golsgqbfa.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvixsybnh.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gyspntjpl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gtvzuzlhx.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gbesusphz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfoymksrn.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/giwbddfqs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gwpcniswq.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gfhqraprx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gjrckwiym.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gsazkqpws.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gbltfgwcc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghbskyjfm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdpahtgih.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gqagnxrgu.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtontevjk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gshputktj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gjtmtlgnf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/goxfjnqqo.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gomnxnyox.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gxgznbddw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gmpsmalbn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gbimvazol.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gkyncnbel.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gsmgluowk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gaatodnlj.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gkvaofivb.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdwshre.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gwqociqgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqexxyral.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gyjglliiz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gybukpiwu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/guwourxwf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gvxaezybx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmupjes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgkzoqek.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gozibxqls.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gcndortgm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gzqxtgkaw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/giqtfjbik.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnzprenpr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzsbrmoqs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ghjfbmgyn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gzstfdivs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grvkcokba.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxirfften.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gltlithka.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gpcpczitz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvhgfqrbd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gvodvzfla.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gpdqthocu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/glaqlmhbs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gshkazjxk.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gcufpdqlo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/glixhdspp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gafkhyztw.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/guflhkiwm.sHtML


<!-- 参考信息 -->