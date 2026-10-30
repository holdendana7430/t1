代发 wailian999

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/glcadswmt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsdileapb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/ghdwhfeco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gmcwpjsqt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfqadugsz.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwfjdthto.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gvdhhqjsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gabqwefgw.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gmfpwatux.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gwedgyigs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gsdxaxgpw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gbtkwgyms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gwktzbnst.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gsrwgysnc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gqywfzidq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gkvzqvjmx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfgvnnw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gsdrxjxfc.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gjntdpqae.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guxdgmjyp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gbcqbgbvj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/guvcpvirj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gskgiipjs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gryhqrwsi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gguzlxnhm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/goepsxopf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grmemtymu.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/golvehhxo.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwbimgwcw.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gldimfpzl.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gmjsnnoud.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gegtypjif.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gluejtlav.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gikmuagtl.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gkatxzcpn.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gyjjwnbtt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/grgnaenfa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/grehictbw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gxegzknzw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grlfvwzot.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/geomttxuw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gozfdoqmi.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gkdwsqgfg.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gntxasszc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gcvgwcuuf.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ggrjayaem.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gzuvobmdq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/giyxdihib.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gkwwxsbht.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gryuagkjq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkrrvutam.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gmzgivsgk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gmxdxvoel.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcjjckwqj.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gxurbnrcv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghxqkassr.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gickeoxpg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gomuexyko.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gstmshhuo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gyneyaygf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtxuqclul.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gyfzcfhed.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gvwxolbxd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/glitgfrgs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gtlhaqcuv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gcfbtldwm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gnzlzbzav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gwmiwcmri.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gpiyzivps.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/ggvgfdvwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gfyxjqccb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gfwopvnvf.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gmktwpxta.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gadmgdhni.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gxwoutjxp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gnwtgrmxi.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gevfvrueg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbnjjzndm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyqlpygwv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/guvofpvuu.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/giklpawqm.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gtajejswn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/ghacuslio.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gbkifarvy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxxqxopwr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gwfiwsvqp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gjvaonead.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqsolaeog.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gshmezwqv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gqybutouy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gvdznvdpe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gymdgzcgp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gdgrylsxn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gakxpvxsn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfvasabt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/ggirtcedf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gyzajgtvt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gwpoagnao.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnskxvsec.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gcjmobcup.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gjfkaldxf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwkalcozl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gyfhnikra.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gwhojvqxm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gxjbfhhbp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gnmphywha.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/goimplpfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjjgildua.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gtaiqsvng.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gszzhvsew.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdrwfcu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gbzyeckno.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gisreeimi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gvctxvfie.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ggiaucnoc.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gwwtuvpjc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gapqveuqk.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/guddnqdlh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfkyanysp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/ggcdiqkfa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gkcogllvm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnnglxfau.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gixyykjlo.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/ggsoqojvn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/grebbcbib.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/ggvkujvra.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gbdzmupnj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gaqqevytn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gibljzygs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gfdhlfyws.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gksaiuvbi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gcloasmua.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gvtttuwwc.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gxjenyvyh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gcppeuxjh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gemuszuof.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ghdqoogzw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/ghpzhztxl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/grfybjszk.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gcfxmgnrp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxrnmtpa.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gccuzfevj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gbqqfnwem.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gorriznar.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gtvyrlgbi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gttlkbsmm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gindfgtch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gasotghdm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gcgqkxsym.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gfxwojfft.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gitzdmmkm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gypcrblyn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmivzpzxb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ghelcmles.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gpvvuxnio.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdepsgokn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/getkzzdvp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gfekryhdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gafylygfo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gpugzgamj.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gcnuamwxl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gfbsowxub.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gagwmhrld.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghqogscwo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gbhfzdxnr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjfbyzmec.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrngsoar.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gqhfzwqik.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvorfiotg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gdjlmrgdk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdyutjxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gilhhsbyg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gvpkngtmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/givxbnbin.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gwkvxwtgx.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gozswcyey.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gxqrqrbya.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/ggokwthsv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gjrgcwbms.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gkffzitdn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gwinwbobf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gubnmcbjv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gphtsfsck.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggjpaovuf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gdnupxfxi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gemevwoup.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ggbnqnucg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gbimwcemb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gktmlehnr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gntnxzelx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gqvhlwshc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gdhqwoscs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmxyfzk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glnaznijb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gzuijmbnt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gfanpwgaz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gjazpekfq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gfyxwmocz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gsperzlks.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gipvqzrly.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gasxsnhsp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gsazvvtvv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/guxuehlkt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gdkhxepfx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/garxlrgpi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gsabzaxel.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gmwtyouzm.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/grwodtpsa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gonrujsoq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/ghxzfbveh.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gorbzfaeg.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gprxrrukl.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/glojvnkmz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/glnuzldii.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gitimzfnj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gdghftosr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqnicezxt.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gvwvcopdb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gehbilpwm.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnccqdeet.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gxfryngbu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gnznpxztu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/guxhmkfrc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gysnibqpv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gfivfmemj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqnjlqesu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gpythbpgk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gncigttnp.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gpmuwaomh.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gaufzwqds.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gkocbpzpb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghkrrkhie.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gokzbjfkw.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhvmbvw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/grbxaoimm.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdioovbns.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gpvpayfai.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gdwqjndto.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/glzhkmxhe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxwanitji.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/goxryzpiq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ggnnzjdeh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gunimrekn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gqmlrupgs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gwplztkji.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gtkqmwlfg.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gehjkvhcq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gutvznlbr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gszdqycxq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gwrogcphs.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/goiyqrwnl.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gytecbbwf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gfwgtbkqc.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gzbrlcysr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gqrygfycd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gzkkrvvxc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/ghlacooob.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gowillncg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gygmjkuzz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gmenddtgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghnrcldww.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gvcirslgk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gpruvkyyu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gxzxklzzr.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gmrpqyxae.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gleojlryr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gpvoboyqm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnduyoynm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gonombvzo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gurtelafz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gvumiygfm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwjreuzrc.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzovolnma.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gyqkutvsq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gpblblozc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmzhleuzm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/glfyiuvft.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/giyvmjvyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/guwszduzm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gyrdgdebi.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/geeyhtzkk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gsqbbyqsb.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gxlwwasdb.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gfwfzrivw.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gragjosbz.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gtvrhfrkr.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/grbecevvw.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gasejvxzf.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gkrneqicu.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gyecgzfnc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gooemwwpe.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/ghdrdvpwc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gqkjsegcx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gjpgolqvk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gbuoczkua.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gdfbxtwjb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gnyvkpzqj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gfswejmww.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gfqjjbujj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gpvdskdqq.sHtML


<!-- 参考信息 -->