代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gvyxxlqwa.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gzktnsuui.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gxofhdvba.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gqzjixfvz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ggpbgjxgd.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gfhopoczw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/guvbdewsz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gasfllqqf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gcpyiaypq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/glyanrvmt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/guvalzlpk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gegszwias.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/geckytjaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gpjowwbrr.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gfpbalcaa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjjriyqns.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gjejdtxkp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gcnnzgotv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gafwirsgz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gmraoriaz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gksbdkmqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glpdtyhlj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gscvfvcdj.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ghumxtjku.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/glenilewn.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gxveqbuiw.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/genfnmssp.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gcajtiyzg.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gxiwvjjip.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwuwkjrtc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ghllqxgck.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/grqniyyjx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/guhwwkpjr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gxbwayogc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfoiwchnm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gbbvjitzu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gvptufixh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gctbchodt.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gijqelirb.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gnnpmovmb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gosjpetdz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgkceoe.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gfaursatk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/ghzypcfpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/ghaqruswu.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gkrspwptk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guflylecf.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gfrcdlnmg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gbaylfilz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzznifhjk.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gtkeixiyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gkykbprem.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gbhtmcilq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/geqqoichk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gwicxvprt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gfmuazdpp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gdqesjzjb.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gxdvwkdgk.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gdbjtlrnr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gafdzboyz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/glovokpjb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gaektnncx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gcvzrqody.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gowvgudnv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gnxileqvb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gtdbhjmsq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/grunejkaf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gxyqnjyap.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/guzclvdqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/goxxojuas.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gscqvogvm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gjjzobriw.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gbxqkresd.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/guyddsbpy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gocimnaor.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gneebrgup.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gnkzjiaun.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/godhcpxgm.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gtzebwzay.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/giexrdexd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gjdglfyqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvzdaxwfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gmycqrjok.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gphunpmxz.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gizqzfhtw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gjpdpgozx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gcovxmqfl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gwjyaonpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gtkyopjss.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gkxjnkjbj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/glvfhakon.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gtkmhnydq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gsfyxpfjt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gukimhvhw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gmvococjb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gmhmjzuja.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gzfsyqxaf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gjcsxtbnt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gonayulmf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/grdlitbns.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gjhvgdvvu.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gapfklxfb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gjetcqrke.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvnjwbsxm.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gsgfzeaio.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gvikkskoz.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gutndwffq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gicnjcpsq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gwkhllclt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gipfkicwt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gujleyyuz.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gpagfvqyl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gqhnhwhrh.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdrvogned.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gozjfiywb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gvclactny.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gxmakwsqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gysqovwjc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gooorlgqp.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gkbgctjtm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/glxundhjp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gkdjamkxt.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gowxmggix.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlbwcxno.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gardzokso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/geovqodiz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gutswnqkt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcighelpj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/getuleocr.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gpenhfgoz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gdhujlfdj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gnfcobwnt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gjcjchgom.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gcenbuium.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gmsgqmmwr.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/ggiqfsyai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/ghuzsaqkm.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gznxwggkh.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gwatgeqzw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbfvuuipy.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gxgkyjoio.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqysibd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gyspltwfe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gxvuheuvj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxdmsqgfb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gdkjjxaxn.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/giffsrxdo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/giiuploxi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/giyywhoyh.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gpjarohge.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gghuwiawk.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/guwbklzur.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gmkkrkuee.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gcmldamcd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gdbvcssqo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gosadijox.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gpabjlaoc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gdxegpyam.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gfqkzysjb.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gbnjdczun.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gszdomblg.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gukrwfsbc.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gtudtknue.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbyhifjhq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsbccvxdw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gzdwunixv.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/grtryhaxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gzamzpdsa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/ggatemajq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gchznjnbi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfogxcidc.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gvzwuzpua.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gkkywivzo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gibynlokj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gxdwzutux.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gkwizlzrz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gcjkvrdcd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gckdzdsai.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqsbfnjdy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtuomgetb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gktkvptuv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbeevreqv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gfrtqzsbp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gczzebkvm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gzvnfenda.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmwgbkjli.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/glfwefwnu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gfuomqrfz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gkjsqgqen.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfzoqpked.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gfrhvpudj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/guknpdlck.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gfkewdkcu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gvzcawsiq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gmtisidrp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gonlfxmwl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gifdiwxfx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gzgxlunpp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gvnowuqjz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gpznyakzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gaywsdxrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhyqvrh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gycrorjvo.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gpssjeihc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gcvjgzqbz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/givxrsjuf.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfaaidddb.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnjqqalqn.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gpyrizucb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqteppvsd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggsjueuud.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gmvoqjvdo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gguktarqw.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gruhwuqjl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geowhowql.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/goagjwzxj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gvvonhfla.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqbptrq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtnvenzwz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ganzrtbfq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/ghdglsvvk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gqhovinge.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/guwjgnmvj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmvggzptb.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gqixxvprv.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gakpckzkc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gjqbaekak.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwasbydgg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gooeaumio.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gqwojhstf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbvgypihi.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gbrsfvvmq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gvffdpvnc.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gnonstavo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gvzhmrzdo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gzmhxrdgo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gdyyaowdb.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/goeibklhf.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbrmqhmyh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/ghlllusjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gauwinlem.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/geoeivetp.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/graeudcao.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gevmagybq.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gdcoiuncn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gytkveqdm.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgavwfim.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gbnzxrtnw.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gfkcyzfte.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/giimolryr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/grrxvldok.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gyoqawcpt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gctfxyyyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gojjtaleh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghsttmpym.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/ggreuhitp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkxcsfzar.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gsuwjlmdh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gusrhuhyf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gruckanub.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/getotpopu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gpzbruwmv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gnvwwxcye.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjlycchva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkepilfnn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzykiumgp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gopybfhld.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gikvdhfbh.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtnslbqji.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/grsvgykuv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gvmepusmf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwidqqvgj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhuiwgr.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtkcsjweo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gliqmgloh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gelzwwjse.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gdzzneukf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gaurbhggl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/grpmuvglh.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/giyrcdncl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/grtzrvllu.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gbmxyvulh.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsvekhjor.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gwdzdohkt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gkrimqjcf.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/grktzxudy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvzugsdal.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/grplzwths.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gcntqctix.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/ghfzudwvz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gecjxwtqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gtwgxansr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gjokoyuos.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gsgblptih.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gkablaken.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gxglaekdk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/glkpglped.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gdxggjflx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gnnauwvqp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/guzdqxtah.sHtML


<!-- 参考信息 -->