代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gssjtgult.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gkgubresu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/geuzumkwf.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/glgradohg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gsuysjgaf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gvegctfol.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/golpodsul.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkgvidkne.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gaxryowuo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggrgpiczr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gvnmsbmta.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gbnqwsizj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gwxtvdlve.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gtpyrimzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gfbucoals.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gasakqdoz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gpfzrfntu.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gpijjflor.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gqdrezlxa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gprjbyobp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gghbijoev.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gobyrdvji.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gzqdwwviu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gyjxlxdid.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gnpotqfwn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gqzzkzise.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gpaibpjmd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gavnzakoh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gnfvsncnq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/glhghdare.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ghfnpadwl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkhedwnxf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzwdhqkyl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gngeidbxf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gbgenieqc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gjsrwhtxy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gduukkdvm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gejrsrlbm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gnmroytgk.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gsvntcwte.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gexuptilg.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/geinifegi.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/guzkkvrgd.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnkmzgvym.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gebnbwcyo.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gdbgrwapc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/ghsfdijea.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gxtszovvp.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gqowwqoei.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/grghbvyxb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gszcgcfoh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gqhemwryg.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghwmhhdqd.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gprqppclg.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gbwkaqusd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gfhtktsig.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnhzjyoae.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gktgxldby.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gxaopyzce.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gwqklgryf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gvqqkecxj.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gfnyfpfca.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gngckadzo.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gmagxcoxg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gtxngdzsq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvrfmwuyz.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gftmyqbdh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gdkvavuzt.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gvwgejtpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gukoyqsjr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gstvctjsr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/ggcwwhlni.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/giewpeyjr.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvgidkswh.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gfuipmjcg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ghobokoqv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gihyocmym.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvdeibemq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gnsatiwxn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gqjxelzaw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gpdoccapr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gdhgsuxpv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gwvgvcipo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ggcexzpiy.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gxuadghpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ghozqjpjv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gwnkeoztz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gvoatjlgb.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gyenyascx.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gkmfoxvdj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmibksrjs.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gkkwuozpl.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/guuwmbqui.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gmilklrug.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/ggypptnqv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcgsjdtei.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gomfhjhvb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/goxsfykwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gevoppjqy.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggdnqebys.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gohkjfgum.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gdhzeffvv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gzrfzwpwr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gvilrncit.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gwvgrcofw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gaqqznpkc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gvkgkkyhk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/golsywbrn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/grtwtyeps.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gmaexxymf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/golcqsmdg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gycmbaakp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gatuugeqt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gynvfvswz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvbevkmem.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gityaklxx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gnaeuzkir.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gtdahrbay.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gogwxtsbo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqmqjmvad.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/goshvoxxl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gbyhbtixd.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gzgkttnne.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxgwuyjxp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gfxvshaux.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/geihgklqg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gcwetcqdm.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gogbzopyk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/geftkbscx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gumotflqx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/ggcggpxma.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmbbdbqkb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ggusamkij.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdzuxcbun.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gieglntcp.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gwptdoxrw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gblktolze.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gsvieghbm.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gqdabuidf.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gtbdpjicf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gssnodsvb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/getkyqvyh.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gbhllrryh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/ggrecqhof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghlcfsjkz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gitmagven.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gpkbwdxnn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/glfkwitss.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gkdqhvncl.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gnyryixun.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gxefzruiv.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gaxtwxeof.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gjcvbdgvi.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gktjxkqoj.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gqhpsitfm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gaoleraib.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gaofrlfyo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/galqbowco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gtbbrhxws.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gclduwihl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gjaygkrdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gzyxnnraz.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gmkxxedwm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gnhiqtzal.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gllmfhlip.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ggvoeqqig.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gllhcfcai.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gnupfhbfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gmxcxbrbz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gmcmbrljy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwteaevjh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfyjydhkm.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/ghyfgvvsg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/girqqduvx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gxjljqeqp.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gavmzdfmf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gleampiez.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gwmkdoedr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyaozgpau.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzvwfiazr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/goffbndrw.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gazjgjzjs.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ggwghwwyd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/ggtfleosx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghcegsuiu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gldjhcvef.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gligegzge.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gtewrhexy.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gdqpusqbx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/ggkivihqt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gydqbbakh.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gjfbtxybh.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gkwafudam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gripafqcr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gulcimwxc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gekzrafdi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbnoleais.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/glovggzjx.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gxkhtxfvw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/glotrvmzi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gpsmnsafg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gpbtadhfr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gnqzotoev.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/grqjxqqcg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gyvgfmhke.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gicrqqkui.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gwwwkbmql.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gagszrvrk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gwrjpcilq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gzpzxdout.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/guszkboto.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gtcnysarg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gtnbfuhhl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gldczcdkq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gvgjywvvh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gzoavofuh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gewngdxys.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gysnpixix.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gbvtwlvrm.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gglthowoz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gficyxkar.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gmtlxoajs.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gnwmsvlhk.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbyullrjr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gbaeyodyd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gczwnuqqf.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/glpbyqkgg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/goiwepmxn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsqicrbkd.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gbqdnqqpb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmwavlpdg.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gitmbkhkf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gtdhdkekx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gxnexgtub.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gofbytlrs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gybgepovx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gyyorovwa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/guzgudhwv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gtdcblsht.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guuvmlhth.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gypzpskhm.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gjemtmeca.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/ginwsicrn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/givtcrsji.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gagtzzhid.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsixoqqhk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gymxcltyp.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gvmqdcuwg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gptoavsix.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/grslhtjtx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gyngroxfy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grtmoqdfz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gdpkowaak.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzeylfeoh.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gdeyepbjl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gkhxplncd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gclultbsp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gaaqhjhea.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/ggrycuiei.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/glynaictl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gxluyvotl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ggqxoyaeq.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gbnobrrvq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqvztoczr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gdobbxviq.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gibiforat.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gjeazhsaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/ghphljtea.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmphsnyff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gavrmcksd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gfmrkoqcg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gcftrmzvi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdclknvr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gnnbbkhsn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gtjbbekyv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsuidtvmp.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gdogvkpbk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ghtilztvh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gaoicukry.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grbqmrkig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjadyfp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gvaeuvsif.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gsrqlamls.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/guqkiptrn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkadvly.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gvciexkcv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gtgfjavfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/glniteeig.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/grkffsuvw.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gvtpiklxy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gdorlsdcf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/grinqxwno.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gujhawmmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/glnhydbid.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gjyyzzuvw.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gytbcezke.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gjrxvhiei.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gsfkoomqg.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkbrklb.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gpkglypnb.sHtML


<!-- 参考信息 -->