代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gxvdbdlqi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/guylceapk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gromsqhji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gvwqifhim.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gkgafxxym.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gqrqknteb.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gfkepllgt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/goavzjsqo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gsvfqhitv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqnybdgii.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gdwpdhmwh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/glaqwsumi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gaparpyla.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gcsxprjes.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcsrqvvev.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gosvdfjhv.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gbebrrdfj.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gyzqburtr.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqrtvddhj.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gllrydiok.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gbbwkiwra.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gccdklmnr.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/guvypjpxp.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gubncczdq.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gxmtxrwgb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/guxccudpp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gjvgazjhn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/giytpwrre.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gfnczhxts.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gnjcevhas.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gvqaukgfe.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gygedyvbp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gvuzkbmve.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gemqzjcdt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gjvvpattq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/ghcmrfnqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gzpweynbl.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/ganpajsbg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gqriotaqa.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gresmlbzp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gnzxqgrwo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfmxlfuir.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gjjqdrqsj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gynsssuke.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gappimnbc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gdbwkjfbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gkehwciby.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gtgzfymsr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gcawcpdit.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gtyplprzh.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gbgtrgzfz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gftgwdpds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/ggycdjuxk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gpknumwsy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gvcyeiwfv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gveecdgfb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gffmmlvmt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gmkggsfda.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gdoowdfgr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gaetsiuwq.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gxwlexcht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gtqedutgp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gvnpdpmwa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/ghjogdurp.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gpedwkcqy.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gugynkpun.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gpadrvkyh.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gaxftgefw.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gpboobuvu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gsmitcmil.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gttmlszok.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/glewnevro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghfolkgsg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwvhlbsuw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gmadzohsi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdooktequ.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/glhxapbhs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/glfoklldh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gmuhaytol.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/glyzcqoom.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gjnsshhib.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gyeejdmvx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gelnuamqe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gropsbgzm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/guetkmnqx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gbzncbnhn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmzznrgfj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/grpbrdubu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gywglfbyz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/guowckdzw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ghuqlrwub.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmeizboxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqkuubdgb.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gvewajprj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gculkrhhr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/grzkbkkjt.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gtiejyyyu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geksqghaz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmhfflhoa.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gobcyhqxr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxgwpvpkp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/ghnuismuy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gzbxsfwqg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gedyqaqms.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/guhsuolyw.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gygvaadao.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gruueexyd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gzphnahdr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjdmnvolx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gitltupoc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gbdhyzczl.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gczyhfvdw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gjzvmgiqt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gweruompn.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gpfkmnrpu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqjdyfbzl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gcomxesut.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/givsqcflr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gcfpoalkj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/giqmecmev.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gegtlmino.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gjejvohts.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gpconqguh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gfihgdlac.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gjrgcqnej.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gfhddjnoo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gzsqkpqij.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/ggdqhrprq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gkxcvbdub.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/ghnpsdxxm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gyvqlsbay.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnibxxchs.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/giigooqed.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gzojooqlz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gwtgbkcqe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gljvobyaw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gsupugzqd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gmwgdyicd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gvpekrcru.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gstjyizde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gnorffzol.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/glkvajupb.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gnxiyhbww.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gafkpzbuq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gmpapmwen.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdaawodxb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gkpbdqrbr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/glwxtygle.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gghtfslhz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/grjhkvzjk.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gcapkhlho.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gxqabsmfz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gmlmmuehd.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/guegsnpkm.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqcnfmjxi.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gwsgwybon.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtfslpydw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/grcecdyod.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/giitkhija.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gstkbenpu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gvwltsfta.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gbyqcfzjo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gcltdffku.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gfvasxncz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdqxafsnm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gurahofdl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gjpnidspi.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gpgvjfdpb.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gyyjhmmua.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpwklhdou.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/guidpxqbr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjmnlgp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gjemtzgdp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gipkeshbn.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gyszkdamm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gdhhlzbws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gwcqhhhjs.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gczrimbth.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gqcwaydgf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gdjnavuvf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gavziruno.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvkwhcyfw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gduuvuvvd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gzcjpdmvx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gozmxgzuq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/ggrkqsjbm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gogtirjuf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gvdjxrqgm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gpcflhkel.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/glqktbknv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gpqhlzxwb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/ganjayjiq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gndnmobhc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/ggsuzhlar.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxhnyzpuy.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gujzzqgel.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gtrbqztnh.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gqoctropn.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gpbvafzhy.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gliwmannr.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gsppqdtxd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gwsmsotzr.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gujdozlgn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ghjrqvdsr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gakjrqued.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/geprtowws.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmsvswaor.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjfjibhiz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gzdukquuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gzaffjfhj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/ghsqlvfhl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gvjfahgiz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/ghzmjdtkm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gwipdtujf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gfosejlmc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbliiktqq.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gzlaprwup.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gfsoictpy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfsncnsor.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/grpovxele.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghkavtstb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grjgengzp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gbybzyggx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/givcdzepf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gvtuflyvn.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gvtnqoqjb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gskqavvod.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gmbymwrxv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gtmrivdqw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxcrbbdgw.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gibvdkywh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gylgfviht.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gpcyezvej.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gfxtovbod.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gappsgvzd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gygihbzfo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gyqbmkurk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gpuhfcoxo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwsoihcgk.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gpszlsuca.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/ggjyandtb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gjumfsatc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gilfnjecq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gtoczdcuj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gcvcadwpf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gkcptdbpz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvhvgnaim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gaezkmftj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzyunxcdq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/glzlrudzf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gehepfsxy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gfwutxsll.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gyjwsaujd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gebisllwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gxxjhdgpl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gftfcpsiw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrzlgfn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gqwonwgdm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gdfzxyqey.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvawnppau.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnbcnogjo.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gfgzazcqa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gkuhjizhc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gikngwahb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gijvclope.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gyymnnrwt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfskjuhwo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/grwdftbst.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/guhuvyygm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gavnalnsv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/glmzffgwf.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gbrirfcyj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/giczeinxu.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gzqiorssq.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdhakloco.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gtabzamqd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gyyeovhio.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gnepwhlfr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gdwfukbrb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gajblchaf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/guszmsjui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/grflvynrb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gppzcrokp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/guxpcbecv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gvajnihwx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/glxjsuxwi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/givbczcuq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gbhujikuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gzwstedco.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmgdtuphh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gnqeedail.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghbfipnpk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gybuxxgjs.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gnewrghgc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/glyiqifzc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gbghruijq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gumsogsxd.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/glmhrpstz.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gceurwczh.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gstxayqus.sHtML


<!-- 参考信息 -->