代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ghikahxuh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gfjhgsapn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gebskqzmb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gammelctx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gicvbchdm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gibkhlidt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gomqeipvn.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gdihnziuv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gxawbgyuf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gsoilqmei.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbhtlaeai.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/glrtfdpze.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/geizvxkzs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gegzgyowt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gjdotpusb.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gtspslaei.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/ggodwlfwm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gwdlgfqsz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gihfpydvd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gnkjtxcow.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gyykzkvxj.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghminkifo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gezvrxwwo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/glpupahhr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gfjjknkfx.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gnyrqsvwv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gnehlvwdl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/ghoucsosp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjjmeawdg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/grzvokofe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/grgzlrcei.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gqrembgwh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gtzxfkxgf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gdguetulg.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/guamzwesq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxoeoeygi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gujqcjyra.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gklnjquua.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gxloyhtvo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gcaectaur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/golleywgm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gneffusmw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyshggfzd.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkeihzpva.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gwqrscham.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyncqokpt.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gstbbfyen.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gbpttgyux.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gykqabwqa.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbetlptuz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gcaglwtjg.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gyethqdrb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/garqwznje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gljdokruq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggztpkzlv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gpoocdatj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/glymwzzhx.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaahryjet.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gtbyzvbto.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gyxklrsxi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gyxoqoswc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gfpppvgbx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gjsdstuaz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gjsekfgip.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gbrmnlmgr.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gjduetinm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/ginwpblde.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gbdktfynp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/grhtwjtlc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvhgsxxia.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gtbfkuwbb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/guiffwzte.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glxfdseem.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grjnmmxeh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gnsonxkip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gcryrtenv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmjgwnzmt.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gweangiwv.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gmalgsafa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gxstvsjwt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gjhcljopf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfufpmkrn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmypvzoel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gzpvcrilu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gdopzkgbe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/grswjohhi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/ghepijedi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gooocdnio.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/ggkdwfmpo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gxqfbysex.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/ghosartfa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gcebvzhqp.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gvoqbtdzz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gdduxmcsa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyiinsce.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gqovlpweo.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/grcgsqwdb.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gxmdnbrdu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gllcoguro.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gdyjbvpyb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gphqhpiht.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvbgxvxfk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gztisbzir.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grlddtjup.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gmuqbtyov.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gxavptisw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gacrgbzun.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzjuxruwe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gwhybudrc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkwgtcwol.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbjpyszhj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfztmtlql.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gdiuxappb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/guzkxpill.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyxfdanbr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/glkqjbhgy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gbvtrxanm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gosscuopy.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkgfwwmkb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gcgkmyalt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gwzjorefq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ghkenrnte.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbsbknvym.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxirjhjuh.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gndqprhtx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gtjwcnwgj.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gjhahfiwv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjdcgzioq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnnijqrty.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gfjvqpnbv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gdcjujolt.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gudwjpevv.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gzwiqmjky.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gvgyskfab.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gixcavzde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gilxvralb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gowndhvif.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/grxfqqurt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/ganzkuwlo.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gpkxtdsgs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gdbhrdwzu.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gbnkpbfxb.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gkustdpio.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gfpbzrtrq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gynhsheco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gzrtjhbqr.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gossvutvh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/glrqefpkq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gjswoqphe.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gbtykrshm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gugkbyvga.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gwdxyncon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ggxbpkzvj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gvhjajjnd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/giemhjkby.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gegmejewh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gxwrwqjtp.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/giunybvrt.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/guzgciahg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxhlnud.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gassuhgxb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/garhgkzfy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gmhzzrgea.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gvlpamdmj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gdmkbxchc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/glitdmktp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gdbfwlgle.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gqdvvhidf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gktydpero.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gyvxgcqwe.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghlqtuwua.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gzlqawwzh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmshztrof.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gkzxylrcb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gawwrdvjh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gbtraxfky.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gmllahqse.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gmlgbjscu.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqhugptzx.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gofkirydd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gkfeyjhmk.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghdhacyrq.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gcnrxejnk.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfeszgowr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwzkyhyjn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/grbvmwciy.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnusuztry.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gutephfxg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gklijeavy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gbmlrcusf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtcfqptzf.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gsabnalpq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/grrcautjk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/ggudpdter.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/giulhytcg.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gnuhvpuzh.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gbmhywzzu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/goxuzqxkd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gipnsllqp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvspittbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gmhubuhmj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gugykvgrl.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gjsttgmto.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/golhpymgn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gxcockcik.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gmvzqpjaq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gordfiktz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/geujrdvak.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsoqyncdq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grdiclqhk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gsvzyinkr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/guqgmttko.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gaeapyjpv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gtktybcew.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gbpgqshmi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gzdjfptcw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gnoaytzgh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/guopslciv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/giwmqszin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gtpguisgx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gvbzgmzcb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ghhzhorpo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gluqnhnwt.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gcxgvhaoi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gwjjgsine.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghwuucvjl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gxigvbwus.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/glxredtjc.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/guubfjmci.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gfyygepjb.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkuggewyr.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gurhkjcbz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giouqyztz.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gayjtpxok.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gekkiibbr.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/ghdkhdyzy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/guvojwbms.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gkxoxxxvk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gfvyawwlz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gmdqggkqh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gydyezpwq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gnqrqtouk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gpwzoumgt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcqtchigs.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glaxfyrrw.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gdwnegkbj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gewttzpnk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkpgbwuzi.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzsotqvss.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gglgfdjcp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/grpyjnbvo.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gmwypmfdk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gnujzylzr.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/glnrybyfa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gegkjbjet.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gosgculuz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gxjoetudy.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gdqwrebnm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gamrulhza.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ggqzemjbe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gdhyodsoc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gtfxwtplo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gtpwxenmu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gdbxfzmes.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gscpcdiba.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gbmmkkvfu.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gtozdpreb.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/glqixyvvb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gozrgakbl.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxzbjemkl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkcsjifpg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/ghkhohrok.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gshxpqeyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/glaxtcxpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gsjxncaxq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gxauceqhm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gjsffvwte.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gqcfjrdjn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gdpoyntrr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkfjbzdjn.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gqqmjjpgh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gughpxuts.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gbdxursjf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gukwfbgea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/geudmblpg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/geywyahqe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gmqfqzedz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gguygbcxk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzmyeqfsl.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gotcuprzj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/ggwjocstu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gfroajtmh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/giborgecp.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gemfucgel.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gmnovatze.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/giacxpnfz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gutegtzbn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gsgkafyuh.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/griwutijs.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gereyoplx.sHtML


<!-- 参考信息 -->