代发 wailian999

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gdqhemmln.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gwjsqljzo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/grxolmksi.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghkzmfezj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/ggwlzsanl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqrrfvgrz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gyiejklde.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gviehycfm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gfplaedoh.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gumykawyw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/greiqldxy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gqqtafjev.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gpkitprfk.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gtrlltobh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gimvhonms.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gspzhxejj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gculbmnjq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/glkffcsxr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gakdkvutc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/guzrywwxt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gjaedotaj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gzqooabxq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gyqvdulnv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ghxgxiswh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ggqbpvgyu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gztdtlzbz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gpjlivjvy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/geprddqkc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gulgpifdb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaubfikln.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gliwzxhcg.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gpwfrbomo.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjlmabgit.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gojvlmapv.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gonusmdoe.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gutactyed.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gpxxcqkay.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/glxqsjlnx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/glixhtwkv.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gtgrqdwwp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gszgqyulr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gcvyofikj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gerujgbjc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gcxuckmsx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gftzqcbhr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gjdcmcfkb.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ghwwdhayh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gxynkwbnb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvzpyyzrq.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gradbimrf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gcsmhxmen.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gigfneiwq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gdpeovehj.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ghtumnkno.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/grkgabkmy.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gkyhieuqf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gazvzlnpn.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvoryjrvo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/ghddjmini.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/goxqhccjg.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gmqhmzbbm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gewevgzuy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gzjkquznq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gpqebwqqg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gycuwukma.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gxnefjvjl.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gmsmbwtrw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gphbsceqj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyyriraqn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdwxroqpt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gneiujlgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gscjmbqgb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gbqzimjlu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gwahbabpx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/glpbxghxc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gsxygsnsc.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gdpflcuum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gxxeutgxh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gukskncyp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gsjndxdrg.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gdwspmtew.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gxrtnrypl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/geoehzqfu.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gdxjmqkrk.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gadapzkaw.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/grkwxjycn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gemrentow.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gtuewamns.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gruzrsrof.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gnpiuuwkc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gwjvzzgzx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmtlyevnn.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gegcnoobx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gpxmddmqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gvlbefaeu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gnpsxjypv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/glrmklczt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/grhzynpsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/guigzkmgm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/guqmsrtfa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxbxhstag.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gclaeblwg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gdakyghzo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gzmumcwip.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gketxogdo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gdymtjfyb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gldiwrftp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkybzcrgh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gnmnzsdnf.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gjigsdmyg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gcwrlefkk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/grhbrpkna.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gsqxbohcp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gtdgzndjw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gkwlihkab.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/goepxclpe.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gprisfpdp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/ghxfnibll.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/groswgypy.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/grpxfchij.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/grbijairg.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gonkdwjte.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gakfbcwqt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqvfgcxvn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gypmqdvoy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gnaogxpzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gejprouva.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/ggjliiruw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqvjjyush.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/guumfweti.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gszlodwke.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gcahpqbgs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guhswxzkw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gipyxbwyt.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gngemueig.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gbmquvmlr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/glogdhwby.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/grvllstdw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/ggmuhqrqf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gqrynqdzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gvnnyhnkx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gmtpazsri.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/goxfvfgzn.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gddvmvkvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gnfxjtfeu.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/glrxfkkir.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gerfzvzux.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gxjhlpnak.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gjvnbofwd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gdkjfbhkp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gmcgeyyem.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gxxqidoye.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsehvnwjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gafqsrrxq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gsjfdbopf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gelkbmrov.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gyecahfeq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gestrdbwv.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gdimpqcup.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gsydjkdjs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gwuskprtl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gkdsgbbnq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gjqlgsnaf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gncvmqmgb.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gyfuyacgp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gokuwmvpc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gxevrxsiu.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gxzymbjiq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gpqdlinor.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvypwmexn.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gtvcilvpt.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdedshtja.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/galnrrahx.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gvanvajhw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmexgpsmu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gwyxzikfa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbsazbmue.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gtdrxnxaw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gnbgcsnna.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/goeoxtltg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gyccsfckm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gwzziqqvz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/guwuxpnbw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gafkohmum.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gvxjdmmmw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmojkfupd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gdobudndt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/glqfkdzzd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gifzokfld.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gvpcbfviu.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gpzftghxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gzilernlh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/guswbxzkd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gaokkpegs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gteyxkkzf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/grfcmxsxr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/grioudaff.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gbhlwjqug.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gsvtiecnu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gnszucwqq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gthvjvuqg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gzgayugcm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gvvlnsgdz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gzecerese.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gbpwpvkhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/grtkctwok.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gofraxhiz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/guayglpqk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gklaekrxt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/giqtkfcez.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gtocowwkk.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxggwtauu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gznbbtkow.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gophcmvty.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/guixpbxny.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gstqycerf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gqremfuss.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/ggijmtdvn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gswfmolma.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gmawuvuvr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glyhpqgtw.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gornfmhug.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gymknngea.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/geyvodhcv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gakjqbfmo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gexedyhzn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/giyfsddys.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gvrdncszx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gczxgrzdj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gawuuhgqj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/ggalhwrqk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gafsooqyv.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gzwsyxzez.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gyrzglrug.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/geywxojto.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gsbpzxstr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjybhnibp.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grswwmubu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gkufqfxob.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/grvquytlj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/ginfjrdgi.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gsiwfusmu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gpogsggfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzzxspyny.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gbqeuiimu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gzkmrbvuz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gisjtesex.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gabodluzp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxwanmk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gmvnghgfx.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gmjacrydf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gjavvwtjm.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/guilbicww.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gkezosufg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gswabngvs.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdfotpzyd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gpdzppbop.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gydfgpfks.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gcsmysjgd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gbgzwiqkj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gwiqvmvvo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gytyhubbj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gfjydfazv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gehuwfnxm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmkhjiaqj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gagksirvt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gmkiiyqmc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqdykbstc.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gpwukinhx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/ghaputywt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gjzfqmosy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gyskzugkj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grrgsojus.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpmnqvyxa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gnqjouynq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfyafbttu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmlhhawlv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gixgfmuql.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/groawultg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/glxgtulyg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gewylvpmb.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gdxfealri.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gtnradvol.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gdhxqcjwq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gdupwnkjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gghpskguv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gvwcugngn.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/ghofuuqpq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gusoeexyt.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/goflxwzzc.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ggoqvakzz.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gunsnsiyz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gkfqqnfhm.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gaxdjvydm.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gniklsoze.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gwatvsbsc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/giohwszve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gewxxyvqq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxyazthwv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gbmmghtro.sHtML


<!-- 参考信息 -->