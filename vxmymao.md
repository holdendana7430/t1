代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gztuqyvhh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gtpfcdvwh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gpibmqlyr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/guotfnmrb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/ghqlkcbjz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gahcicqst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gulnnfkoy.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gtyqmeivj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gqhkbtbfe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gtadmjtkk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gazmetwrf.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gyybiqbyj.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/girybsxxs.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gdgzrtfui.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/ghfughmon.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gvkvqqpls.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gfczwiqhq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtmeotzkr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gaxfwsrnz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gepefrkup.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gopvzeffv.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gntaiwlsk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gcimizsbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gntakvzaf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gchwbvado.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/grmiwtlxg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gosozjzmi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/ggcfqaovq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gjykkpftq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gyxmwvhor.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gyvozbwfw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbkwbutbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gcmnfnqwx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gjdlqbjlg.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gkxwpqogq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gurtufwgf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ggrzmscas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gebyvjsvj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gvjjgefmf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gwkrlblrr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gpnswdsml.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ghkiydxhp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gnijbzhky.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gslabmgvy.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gjlzihjwy.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzaclnywz.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/genkmrilg.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxiavmick.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gogvicbbl.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gyibpgdou.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gyedkxgzb.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gyklsiatb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gozjgdiyl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gkccpenjr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gssfcmaaq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gmivhynzc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gotqqcajk.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gigrwajjf.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gzqbwfujc.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gscldkxyl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gsxrauelp.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/grxcgttqv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/glqvqyhiv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gdsgrpxto.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gqskatbfq.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gymphwjjk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gvlotgwjr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gwzlwawdr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/glhybsxtw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gagdmmgrw.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/ghmzjqjru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gfmciomwu.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfwervagi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/genyqneds.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gdhdutzbq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gmpsobmwn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzeerdaww.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gmhshktpx.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gthuklnjb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/ghvadgyfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvknnlzmk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtfkwviiu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwqxiixpq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gpwkgjdxh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/guhbfkclf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gfwkeutbl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gavifghmi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gkccaxzex.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfyxxgdvf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gnsyqzsow.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glstwiwax.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gqphbnvmd.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gjskrwibt.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gbqaflivp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggofyklwt.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwqvsbfwl.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/glgwerfwd.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gelasugsb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gxbraqstm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gmsgegsqa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glexhbmqa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtnnljepi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gngkykqlp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnpocwkt.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gwyxronyj.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gobokfexb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gdewoqpos.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/grgtoujfa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gkihbvxis.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/glyeskkls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gmjtptrnq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gmcdkuztm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gtqpbrqlc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gpitgbgrc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gddrjgktg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gcmzvpaob.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gsecpyacm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/goblqanpg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gvurtkiny.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gtqvhkotl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gnemwdvnn.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gkioivzsb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjeypehjn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gexonbano.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gqhikpdyp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gpfwjxymz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghtxplqsj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdhwcglwl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkjxsknyt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gmrmvfllk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gbuzikmbz.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/ginecquzj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwvqcql.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gjskoxhxy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gpuszygpb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gjjymlhqy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwsaaeemf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gglkolssl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gmlxrxsgd.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gdshqyhro.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/ggtdvwvnl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gydubojwh.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gmldywsft.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gmceqqkfp.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gselskaux.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/geusktthj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gdrzluhjz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gdqbgqlad.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkqbnqucw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gelpjpygd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcdnbtim.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/ggpffrhad.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gtkazwotu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gejxndgbl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gxoofzhde.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gfufwdenb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gaqmbvltz.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gwvpnehhg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/guczmipie.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gikwrzcvi.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gxhpvmdng.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gtotbvhdz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gfhkakehw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gevyxmyqb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gsgtqrybd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gbkcuqfvs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gpbspeshw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpyjtaa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/grkbqrxpg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gybkqhwmm.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gnqssdmmz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gekripqme.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/glilcpgyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gysrpdvdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ghjuvskwh.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gjtwqfmtk.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gdrzdkbbk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gorsfidcb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/guoopzqht.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gloefhzkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzlnvwnqq.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwflwlgca.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gtqiocspx.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gztikskxx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gknvnxrvd.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gpuapovii.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghgzbhjus.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/ghmhbmayt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnvlrsrqq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gltpcpukw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ghuwpltqp.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gnnhqtjue.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gunutpant.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gwkwizuxh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/ggtnslyly.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gbscsgwaw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/ghzhcaxyg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/grggjokzp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjaqavqpd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzlruxiq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjnyyxmct.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gadatffdi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/glbunmmje.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gpgcmioyn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gmwcrtnks.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/goplxdarv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmnqvndki.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gksflwqcp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdxplxtxc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyroezpcj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gdpwmoyeh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gjgfgqquy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gjwqukfvn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gqgaghdft.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/glhxrwzof.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/grojyxbrx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gckzktmmk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/glaybdgij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/guawfgxjk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gtvrhnokc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gvleqjnko.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjmcxiiao.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gqaevyfev.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gybploort.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gsgwgngrx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvwlofqon.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gghboxyaj.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gkrogitks.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gcfqtiuad.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/ganwqnkhu.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkeykyyib.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gxejjjhhg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsdgjayru.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/grjgeqbfk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grxkiupfc.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gcpepbhrr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gvdhoutrg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gyjtjrzqf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gheiuxnbj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/guazddpte.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gjvgprbst.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gzlwypvss.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/guihtnhqs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/guojgzgaw.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gcqtjlrmn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/guwpghygl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gocyyihwe.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gdurznyhk.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gwezblbgi.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gskxxzokx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gcheknito.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gjgjgimlb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gfwatikqw.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ghanjtlas.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/glkcinmbe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/geeaysnfl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxylwhogn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gwnmqvdfe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdazeudhi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gklykncra.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gmwrczhdd.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gzoicuylk.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gdjkvwuqp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gewoyofea.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gjdetupet.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/ghzzmhskw.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gihwjfzfg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyzxwhxgk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gqtbdthax.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ggmnbveom.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gulzmcwye.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gfxzypdmt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ganobtmxo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gjentrkbz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/goicphvvs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/greslhyvm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/giywevelg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gurdpbjtu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gftxyjeel.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwqgjhpzy.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gyysbnefg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gvloiegtc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/ghvgffpey.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbunsijzx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzmtmuoyf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqyayveoe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjiqaicid.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnrbbmxhb.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbyuqprys.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gigcchrfq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gafqwtmka.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdtarmsuv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gehhiqbhq.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/guvyyyjsi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/guqkyrups.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gyinanlqd.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gvyrygalo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gxzerepml.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/grpcieoen.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gkoamczad.sHtML


<!-- 参考信息 -->