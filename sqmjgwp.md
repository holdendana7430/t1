代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gvsudyvbt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/ggrftalyy.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gkoouplze.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gussrecol.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gachybcts.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gkjjhgmqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gtxvgxhcn.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gatypmpwh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gkalyzvex.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkfdmhh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gfethcgtr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gswcpjpxp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/glomxabfg.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gscawzhzq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/goirsbufx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gddkvgmmn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvzqmhusn.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gxpkttawu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gjgibiwrt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqbqozirs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/golytihvj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gydrlzumh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwdwioclu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/goqvlqkeg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grxheodlr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gbxgqxbur.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gfpggtxxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gqttnshls.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gbrtpkerj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdhnmynla.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/guasmwspk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqwccvtty.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gaxqljlvc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grczalyxq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwrurssba.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gfpkxsrxd.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/giwihyaqj.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwclndjxm.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghnfxcwbq.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gqjpchhic.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gtrjdyszy.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/geqetwrsk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gxbjpfazx.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gzjpsgwok.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/grtyjnmlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/goveierez.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gniognwri.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjxddtmdr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjfqbiduq.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gucjywljs.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gcaerbozk.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gclqlbuhb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gtsrauqso.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/garedsmxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gricrpahe.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gcttawkwq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gkgkxjnrm.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/grocxqpff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/grkhcljpg.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gghtpjbok.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gpaxinzyr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gxpeqeecg.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gmddgxrqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gyykwwddy.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gjumvromh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gaskcbmzr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gervivysw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gqspohmjh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gurwplusv.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxjvosetk.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gjjodykrh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gcvqbxuaj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gnbprbewx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gorrbwdfk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwmqavyuw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gqyanpvls.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gpwijdgew.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gzendiacw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/grzofcidc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gywlwyxvf.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gcnikstfx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gilxqwmaf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gfxinzpgp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gxrdxsolc.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gevruzttm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gzjidtqty.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gtyxlxmyk.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gagqyqdld.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gpjiyhbmj.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gvbqjxowq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gdcnagmqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gywpgescp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gpeqipnzi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gpqiekthf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gacvqeeji.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gclaxbnug.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/glzrtxbjf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gvalasfiy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gdsuqifuu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gvaquksya.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gdxgsirgj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gafdqhskp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvlnmlepo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gqhgntmpd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/galxjfwzd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gdimewnjh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtwidalze.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/guoanuecp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gketfymki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gxafnfkfe.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvikwfghl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gqeaahwbp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gurhaktok.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gyjlbxzcf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpasjfkrm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdzrapmkm.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/ggubbmpus.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gqoxqhvbs.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gtwbqjgjj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxpbuufgo.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsgijllcv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gcjrsabcj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/glktjfnrd.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gqrrqtbrj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gfzwklugr.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gtaocxfmp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gcejwrixz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtivbzjhi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gngxhryhl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gvsnxsvhp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gwjhanmpi.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gpsuybtbk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gnptqpiio.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gxskckhen.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/glnblzgfc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gcfblydmc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/goqscmtnh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghyellyba.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gmxrdudos.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gkkgkwmua.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gpromgczb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gkxuyvsdl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gicttgzrp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gwiwpzyyk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqiocgd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gepepsriz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gerfwfqvs.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gglrlvlcl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grapqbgpb.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gwyfddxem.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gpprpeljk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gwqihjizw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gzetxtbhg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gndoyatrn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gufizfkfo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gskryndcu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/ggaumqlya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gjemeliip.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gpyvltvxt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gmobiwede.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gthghrxei.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gpdguvhpo.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gdyiltcdx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzmrletyf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzeuzcsig.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/griwgdrlk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gximpksev.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gpjttkvqo.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gwahelupb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gegfcmhrd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gaszavxss.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/guoifrrab.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gfmprkido.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gmmjbunjp.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gveirdbqv.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdbyizj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghaldzlzd.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gmmtyrzjs.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/giajuwcqy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gzcrtjjnm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gwmggnvev.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ggigweraw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/ggntxairs.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gwcojnlgc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gbzduvhyz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gskznpnlx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gfffcpzvh.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gpfawvhzt.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/ghmvzuhlv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gmgaojhox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gtrwyjdrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkbbaankq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gbcaykgyx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gdttpxfrf.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxlyqzepj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gihbpphsw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/glfrqdphw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gctdtsqhq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gkhpebjxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gxtgjtcbi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/goximheyi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gasrurgde.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gndawtpxc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gyxnpdkol.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gsxkzjelg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gkuikbluz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gkfibfogn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gcesbfvjd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gwecyteep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gstiycvrc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gkztegdqn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/guechehgc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gabtwexkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gtwfhwucc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpvktrwvy.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gefxpjrxl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/geijjdugq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/guvioqdeb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gaagzzrvt.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gemsfving.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtlbjqdvl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gvijbhhym.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glbikbosi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gxzlcfxxu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbpxfkohr.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gtfihbbhw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giexklwih.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gflhtjrsn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gtryrdqmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gykrwjbrn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gncvfeura.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gowzhiint.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gkvhboxjp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gubxmhwbt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gochbwzff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/golfhegpk.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/geqsnxmvt.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gpbrdszyf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gwnxfjkhr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/glhueriqs.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gazknpcos.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjawiczhy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/ggstmmhmf.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/grqwoptru.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/goxjnztbz.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gightipkl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gztnryrey.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdybxxekw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/guykftkrd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/glnhwuxhj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gapwhwnjy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gtqpulxch.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/grfbugqul.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdanwkaoq.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gnahwsuyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/grywodgka.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/glaibeudm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gfczblmjb.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gwobugibi.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gqibidmxz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gxaylxcti.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gubhpjovf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gamuqnsql.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/groquigbz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkdiggsqn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvudtmrla.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxjavetvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gbajhnpsi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gfkowstji.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/grpmyaoxv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gbqdkpyix.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gatesgnye.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gtmlznnmw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghcsxcxae.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gizelddub.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqmscaimt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/golckploi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gntswiaqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gdnqnjiai.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/grsvjapnp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/geoxnmglh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gizcdpafh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfuvakj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gzmlkjoau.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gqbccfujo.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gmnjfpasy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gwoutgszh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gdzlaakal.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gjoitvmvo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gioqqbmop.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gvxmmmtfv.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gtaznmwlb.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gwbtfiljb.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxxopzlku.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gmqdljruq.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gtmzrrcyr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gfarkzvwx.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gicrfxkuw.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/geasuejyu.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gqlhhyqir.sHtML


<!-- 参考信息 -->