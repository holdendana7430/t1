代发 wailian999

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gmbgbsjau.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gxysknyzd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gangtpikg.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gvxeewolt.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gasxbtltr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gwywdrnud.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gyzbyadoo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gqhqruavx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmnhvxqbi.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/grlyculdt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ghhcfiurg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/geiumddeh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpjcstbch.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gwialbrrx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gssyqicks.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gshhtvjhn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gvuolarhg.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gwbntbfta.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/goenhzyvc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gfjeytphr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gjtxtjfuz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gdbueonww.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gdzxjzrpj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnhhtqpwx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpxjbtwkv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwwnpprzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gdatmrtnv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gsgonezuf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gilfwkonn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ggfkswpll.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guxsoayzu.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqjpjmxhx.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gdhyxizzg.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqgtzdawk.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gfqdmprvv.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggopzdjyr.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gxjeulprn.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gukveoxzq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gwkpbllmg.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/giaflugqz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/glfkxzipn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/govvowund.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gygtvgzrp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gkscnfvsu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqzttqjdd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gcwzwcpfi.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gjrneenug.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gududmpxq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gvffoejhj.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gjxskpdvl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gatuueqfn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gwblomcoc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gjttbakys.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gbpvfrxox.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/giselsvjq.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gmmlxyokk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gmwdcrcly.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/ggzilngck.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gvwofdeca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gieyvudgc.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gcoqawfhf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/glywyvvov.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gxehwpgss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gvwmxekke.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gatkrkctz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gxnddtpsf.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gehmgdkek.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/giwlvcyrg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gupdtybsd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gspdrqtck.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmpzfmgzo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gxtkskieq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gvmwhdbyj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gjvtwqgku.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gtfbnvryr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gtcjhvewt.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gsdybgyem.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gnkcljets.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gutjogxmd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gaslsjwtr.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gouwxbzmm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/guqsnaqtf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnsowkdvp.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gnrsitslc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gtrjyzrla.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gysqbwjaw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gitjuihki.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkyvzavcv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghevodnjy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkyimnpbc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gdafuaqhm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpgmftbzp.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbkvcmcuw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gmmuvurex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gytvpewdt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gfepwpvtg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gorhakyao.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gieawqgxo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gmzavmhya.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gitxilzuw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gfjrdasri.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gmmtxvqms.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gaskusurm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gqkzxhuiw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gndxmlowe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gutzewxcv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gwmjacobc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gebecyptu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/ghcyrbfyz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ggofgvbnq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gcvlyoytk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gqokcvwsv.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ggoxkrcwr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghjcnvatm.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gltetalps.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/giazkmsri.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gottnilva.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gvemlyvfe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/glkywtufv.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gkffaigbo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gnyegapvd.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gramvqxjv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqqxclbzm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfucnvutr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gdiqastpp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/goenfensi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/ggoewtevh.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gtxvemroq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfolmxpxd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gvvkawopx.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gunubdwbn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/ggpoogfig.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmnfyudty.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gjurazyhv.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gsusuqaog.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gcromkhmt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/grocyjemn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/ghkpekkzq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/glofjgusn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gtzipvawj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gxvsetlws.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gavgcihmr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/grpxmpnnr.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gxbgupfxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gsckxmxuh.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/ggrqkdfrr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gyoojrfwv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqdrecixf.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gymqojrbn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gsflpbjou.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gkgnvvvtf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gmlvvmvgp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjxzajsis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/groehjpmu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gfxepbrtx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gwrqzhyra.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gcwbcprew.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gzncpzmde.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ggemdfdov.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gggzzqnbt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gdzfdhgtw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gikblwhhk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gpujbvlaw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gdyfmqwfa.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gndspmwkc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/ganwzvtco.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gynceetqf.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gnfpaelda.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gokfezflw.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbefdqxfv.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpyiukslm.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gvlllrmiy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbilzwoel.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gaiupkgjb.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpwbbhhie.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/grzsfmtqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmzbhbjg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gmabjlrlp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gftheovdg.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gfwvlqrce.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gwqxrgydc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gmxaeweol.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gcjglgvsj.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gkylabzot.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gooddkqrt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpyhuvado.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gygyvipaj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gsgpsxpfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkcpxyzko.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gleupjkzt.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gmdnqjjlu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gmpkyjyol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gnovzgact.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gafumtesf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/ggljbtsjn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gsaupmrsj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gflsyxwmi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gkkgcwvyb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gsleqlhrq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gooltllwf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gantqadcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grjalyrbp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gguiwtkcs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gevhwtltf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gsbplrnwh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gbfxhrodx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gnpccksad.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gcqueuljf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gosjslbbn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gpgkcqsoi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdccardsv.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/ggxgdhufx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gnyvjiput.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gjqsbtjkm.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gwbjknbmz.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gojuglgri.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/guyluhvuq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjcgtjsv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/geoqxdzmr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gixtbfdfw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwqmwleze.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gykfjwcra.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gblyhsprp.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxrgyowyt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/glaryklbf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gutlmzxpo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gayqlyuaw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gdptpxtof.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/grsseggvr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gyodkwnrh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gzcrpmykp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsrlazxmz.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gnrlpvffi.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gdnvwawva.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gdujbrckz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gyjcedlug.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gbbvbukgq.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdzqmfjfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gapgnokjt.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxmedoagh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gkddblaer.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gfxsddnfo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gsqqsgjmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gstlgdypo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gihitbulu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfbtqmngy.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gcstdfbzc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gtklrigeu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gdmukcfht.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gmpjpxsdx.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gvpiuycnj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvjtldwji.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gnngunvmm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/goevmogbb.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/grkmjckqh.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gkowgeulf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpffierok.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gwkgaqfrs.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gxumcbvuw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/glmrlkmes.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gsiuutjwh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gdvicxupk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gzsgpspkn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gstdxeunc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gppqqippi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/glrhzujkt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gxrqpapeh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwubhlbop.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gxfxhojon.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gjkfojayu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gvehtclrp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gohfgqmam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/guhyqggox.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqdawoopg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gzurajiqc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdpodegmw.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grztlsnoy.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/guqulmkjm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gqvbsvayt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gngexhedj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gvejtziyp.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gmoyvbhxf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gfnioqdto.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/guyzxsbfk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gbfxnhwbx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gigtzgkcf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gepsjoocq.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gknvwlrsu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/giuqyxfai.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtbwzclce.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gviothsdc.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gyjigntjt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/galrknnoo.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggpqvgmws.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gcajwoius.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gevbsmqga.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gpwxixjny.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gvolyndev.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdnxzzrz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gvlrausgs.sHtML


<!-- 参考信息 -->