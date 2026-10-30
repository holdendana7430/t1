代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/giazanjyl.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gfpobmxtx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/grjzhuklx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjjmbqrxw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gyaidgljc.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gxpmsznau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gncoafjld.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/geyupocie.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/granyewbf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gthtsiova.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gnnugbqlv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gogrqkupw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gchoicrjs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gnlulruzf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gldkqaqve.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gvmsgewlr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/glflqgfcw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gmkwywbcd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gluelhqpd.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkplumqwh.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gbiwrtqae.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsayomici.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gvmmzbsdo.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gifoahhbr.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gixupzqxf.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gfnlrljej.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/glgeezuxb.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gjsivqmse.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gvblpzpnp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gyaxtxlir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grjpzdicu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gcrcvcvui.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvvhggsjo.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gyepizidl.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gaukqekdz.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gdlqcvnxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/giprlwzow.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ghprjgekg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuznewt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/glcvjhvnl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gspzhazpl.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gafdiwhpq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gfgvumtzq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gxftgswnp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gteimkgyz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnbcgovxe.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gpzefvslm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gedvehrzy.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gmuhmojbd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gvxgguhjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/ggysstowy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gooeddyig.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjgnxolwx.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwmxkjadl.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gaycwufbr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/grrgfbhxm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gviyvbzua.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gzaumprsh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gssczqqvj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ggkozrcbd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gmovdlbsq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/giriwgiwk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghtayexgv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gekeudbre.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gwrotlzsx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gjadqgjxm.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/galexjzzj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/geowubvgs.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/guwirevsw.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/grilfdrbn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsbpuxmcb.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gpidrwvel.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gsjxiiewv.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/ganjbhpzr.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/giczjqrsd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gbqsiqkhx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gewbvrbwc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gsdlqwejy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/getjiyruo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyoltidpf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gmtydfjyk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/ggxranmku.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpefmsxgf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gqjnzbhdq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ggzjswzdy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gseoxbjie.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gziolojzj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtybanwvq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gafkutita.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gpqhbdtps.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwsxfdaue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/glmprvkfw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gbbgzvcin.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gxsmvoern.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/glvjjrlbe.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/galpmwpwx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/ghjzsvpxe.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ggkdntira.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkpguzqrm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjqmjqnmj.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gszjrmlcl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/glpcyxody.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gcrlhsnun.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbgsmaozc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gsruawich.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gvkkfewlj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gpieakoat.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gaeopmoyf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gdcegervy.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gmwoqqaqj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gapkoojxj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzhowkfx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtggoqceu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gaoaulftm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmneqjnoa.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gqoxcutaf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gsyopgdbm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gdhunteqx.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjnmqrymd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gqtexuytv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/grtwviugy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ghhlscvmt.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gcyxqwbpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gqumvpvvd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/graooajkw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/guvvwnmtu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gukmjniuu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/ggldzpooz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gxxbnvkuy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gxyfoxuum.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/giwvkilrz.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gtiqztygh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gayzkdzvj.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/grvgisbbm.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gohfopcsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gssmlntym.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gwhufehbp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gwnluvbay.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdggdpn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gneovqodr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdawfjppl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gyjkszoke.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gzpopxmll.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gipdotots.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/ggpnpzktv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gtvpahrsb.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gzjfympqo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gjxsqxvke.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/geikztvus.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gakwexggo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gsibmcphc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gqqdfdxxw.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gkjisijkm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gzbnxxmqx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gslpvbugt.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gzyzxoxfe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gseokhnnw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gffrcjpvt.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghxamkutz.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gharkvfkn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gthvrsihm.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gvnumjqyl.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gszsyuisl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gclaqhuyl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/ghesnpdlm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gioouaaha.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnbvakfau.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/giyuhhhyj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gvuopyaoh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gxmqzompe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gayhiyukt.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gokixjqyj.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/ghitxwwvl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjoticlqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/ggfvlocxd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gxfmxgwuf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gytgkxara.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ggznieope.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxqtxchhg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gcnwymlhf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gmhpogumb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/geqtiapdx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjnbxosoc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gfjghljdz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gdiwbapvs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gwxhpzonk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gnhwzweou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtnytsrev.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gpsojjvre.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gztryuyrx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/ggyfuufgp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gwzhamfym.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gcdmoiwww.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gnnjluyov.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gcvljvopw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/ghnlhpsij.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnskdrp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gbihhxpcx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gxcyhmyhv.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gkjomcway.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/ggchoumzi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gqxzubwwo.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gnyizvysw.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjkxhbxvl.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gttytwiob.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpblpurnm.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzsapcwye.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gfluhdrbf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvjwqmhsf.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gcbixrkxd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grzsqubwa.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvfxtmvgo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gquszhdza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdbxyozxm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gjkdithao.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gcsflaugc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gglkoscfl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gowitkuay.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gmaefromo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwzeftdyh.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gxvpbwexn.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gdnaqxnyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gfsabyrpz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxchgcxpt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkimkdcxs.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gkcncitdj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grdtfxdza.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gpoywvemi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gcxbsmjgn.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/glfxiuofx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gmpncjcoz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/guiunfrdg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gacwmvvsy.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfnepes.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gojshqnyk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gjxdydwss.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gpjzgycqg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gallnjnhj.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gitiilpkp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gfzplthrv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gxkkqusbg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gcotbglbx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/grsgmjxil.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbjulxepj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gxmglmcvv.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxklpgjer.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gubsizpxo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/grcwfvsni.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gglamqnpo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gxndikwaz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwvxqaose.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/grqovwpaq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfykxyuss.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gemiwcjja.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/goaldzvcd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxceivjoq.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gelctsmcm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gqowbjwvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gmlstooei.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbogdqa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggmqayxxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpbgcfpta.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggwzsftao.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdwtalvdb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gompbiizh.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gamnptmfq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gtxdgmohe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gaxrgcfvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gpyasimov.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gelozlldl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gdsatbrqd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gzyrgmmcf.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/glrgzaylo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gnycqqrzg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gyepxrkdq.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gjdvqrnwo.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/groajysrg.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gnispgdac.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjhermwqy.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gashwzpeg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gvtpzcahj.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/giocjzdrt.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gyjwvxbgx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gzsadvdfu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/ghcgvcxle.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gksaevhby.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gsioqwfvt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gldsjqfbf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ggxmzsngv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gcesnzeyl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gubhbhmqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gkrkutgsi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gadyfjxii.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gntcjlahi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/guanngejb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/glykdufra.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtmpxwowz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gxghokaqd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwgeedxro.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmplrtudw.sHtML


<!-- 参考信息 -->