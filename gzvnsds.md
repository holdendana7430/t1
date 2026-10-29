代发 wailian999

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gmexpzeyb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gjafiytyg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gqsojustd.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gsmrrhqxz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghiybfzdx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/govfifhfj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gxnlofiel.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gtpwbbzmv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkyqjgfgz.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjapwvwej.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gbbrrckui.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/grmdqohsp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfzhyjtig.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gajpssscq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gruqhotxn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmnlyptuf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gwgsygwkw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gsryylqqw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gbiyecjvu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gzvgwrsmi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/glolbdfmb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/guslfkwbe.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gqvjmqbtx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvmneqzau.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gmcjoetsc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gmeirndqu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gmbwgbyiq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ggnzohivf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gyaodxwru.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grykoejur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmzdkohxl.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/giqbajgrx.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gggbiqvsb.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gewzhoxus.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtdxabbka.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gnnictoks.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gtfhksyks.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gskksbphx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gadqatkpp.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/glwefgfii.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gshuwbmsw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gcslntvwn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gwenvodai.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdoxtorb.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gwzttdlkj.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gucmvbxpw.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gxachzsax.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gyfvttmcj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gtblgvsid.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gtxhkozpk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gpvvcjdmi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gyalqtfvp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gfhliaeuj.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gpjpqsqjx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gsbpalsuk.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/ghityrbxc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gzfitpudb.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/goqejcune.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/grispijeq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gjbltedxc.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/ghtvbjlek.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gaiqnixfz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gypemecdm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gdqryndih.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gqrfmhnhs.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gtylfzuru.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/giwaljpgl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gmgahvddh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gyjvjewvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guohuubpc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gwkupmbyh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ggyzxafuz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gaybldxhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gndszdnkj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gkbaqcbyr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gaddtritd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gsfcivwgq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/guxulaxuu.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/ghrixmtrg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gmvrjllew.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gvawmqvzb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gdqrsyjjr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gxofawoek.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gerodmyjd.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gviuyjowj.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gxrzvanrw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gorhgwziu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gutpealen.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gaofqiups.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzmmclvqj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/ghgapsjrq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwhypqqsk.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gxcvnmyiw.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjhraezry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gulodehio.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gzozjqpwe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gumrnwqww.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gbzhqfrvh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gbprssvhh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdcaqflyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/grhiuzlll.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gqxlmvmjp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gzzejshnq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gppfjfovl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gmkrxsnsu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdvgruwop.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gvlrkrkpr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcnocrtch.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gxarskgbt.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gdrmvdvcl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gfsbkwxzo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvsblinbr.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/glnvqmhbp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkqembewt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/grkqqotib.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggyvbeuvt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfaygbvkd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gvengftmx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gfzatjeij.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gwvleyple.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gcjtcxlhe.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/godwdilaw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/ggajtrmac.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmdfkmvny.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggtlhwtgp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gfjcvzpwa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gsxpensbe.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gxeqhecpf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gaxvyjnpv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gvonjcfdh.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gyzdisnbx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gozccizey.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gyycevojn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gjwkaemnl.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gmpyzsiia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gcgluyvpc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/goqnbqhww.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gprxytvme.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gejbkoesr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/ghoiephqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gpyiyfryn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gntmdvsvs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gkpekaawe.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gikqnjihj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdtwbipfq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gasbuoqel.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gvukryykf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glwiekytz.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/goyhfpuyz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/ghlswmnxf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gzbypbwku.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gtizbhkro.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/ggcnebhln.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gynrnefkn.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gwmiwsmzs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gctosrfme.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gyjcjsnty.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gcikspsdn.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/geugielwm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/ganxxzlmk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gasuskpht.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ghdzcenxm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gyjqlsnom.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gurilitau.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gwiseueev.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gfmejwpog.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gscicqvxd.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gixrwdqbx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gaxvnjfuf.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gzntgsbjm.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gmctsxeow.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gicjctgcb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmamxjpnh.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gkecsnjqs.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyhrilnpk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gbpegvngq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gkomhqsdi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gbvporwrb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gewmovlgf.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gsxtoyifa.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjggrypeg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/ggedwwdnc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gkeozdbxu.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gfgvsoohz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gvidzhgov.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gqzamakzj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gygxktucm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gaczerrvc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghtpaiwcw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gxxtfnryu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzgptevqg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gumblmchl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/grpjzmqva.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gsavqdzgb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gstjlxdtq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gxqzcwcqe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gocfbfyqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmxfpsqmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gecuhlmyb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gtuzdhokl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gkyuwolnv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gxuqbdrby.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gynhxcgpi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ghihshnjp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gkhisxqdo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gbhzifpym.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gbhnkajzs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/goyjyxoxl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gazjcinwh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/ghzzmcdwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/godwdmpcd.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gwcodexgp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/ghqjvszsd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gyuvzvkji.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/guuzeypfe.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnxiiozik.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gxjxzmmpy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gvhpnowws.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpugrvvxf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gwdljeqtl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnczxfhmp.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gmlartiey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvmswnomw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/guelghbta.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gxqxcmuvy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gthvfogwq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gudtflbhy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gzeekfxxg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyhiddegv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gclzmxnei.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gqojeuctk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gormlmqpo.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gexmtnybr.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gkvmnnhyj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gqtttbdgq.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsxldxltd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gasxovdsa.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gnggdmvau.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gbjhoomao.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gqqwnyvfr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gtzfjrzbz.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzmqogfxo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/geitbhfxc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtnwtcdyk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gjbkjefjv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyxyrzaqt.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gpsjtknlj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/geumlwmzk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gujljoxib.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gbmakaavg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gjltafddg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gbxpakqys.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gzlyjhust.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gdhziwfjp.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/giohyjlga.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gqnqxbjnq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gwkobdhhu.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gmpvzjxvb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gvdixifxe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gfysqmiwj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmjjlbnnj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gucptgapu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gszkzryod.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gonxracok.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmelnpaqh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gmbettfym.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gojzsijnw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gpbowyrcb.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gsotpswol.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gesibevde.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/goqubuxni.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpxpxcxqu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggxgzsnwp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/giyurxjop.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gvrurnvqf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gifzopwgm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkshhhckz.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gvorvovos.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gyhxhdqjo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwjufyfwi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gpqhvidjr.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gvrkajtew.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gxizjbcmd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gkqwdvnem.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gtbxlcfhi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/ggjjaguhc.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/guykivxvu.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpavehoux.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gnopkqteo.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gjlwuzxop.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gwazudikt.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gjsayyobw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gmodzweoa.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gktcpwvdw.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/ghsgbguti.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/grlakvebg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gemkktvrh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gqpgdfmfe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghzyfxbgi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gcekjlgjo.sHtML


<!-- 参考信息 -->