代发 wailian999

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gooudkqot.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gfppddjxu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtijmsde.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgixbdt.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gidhanymr.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gownihsji.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gvoijwzux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gvctzjtln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/giwpzsjgn.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gigjpyqvm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/glsonqzqt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/ggcncjkib.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdeziturc.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gwsebjcxh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gcptquxeb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/govgtlydr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gsrsitubh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gclmqewex.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmdribfzc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gowgtingo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gjbbriaqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gyiusjith.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gjynydeng.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfytbzazy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gqbxvzgrb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gflgumqls.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gtdbsryac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gdsbddxfp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gpffczrvh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gsfrriybc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggaelmzdm.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gahvswnij.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjelyslrs.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gllfklcun.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gkugzabsy.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/ghfqnzamo.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gmmmdhctq.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/guuxttzrk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gpppjmepr.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/ggqsjtlgz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/golovxqyx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gepzslggt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gjtknyvnd.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ggataxmpq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjsafzhif.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvnrnboas.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gmolybmyo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdeluxx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcegagb.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gqxhynitn.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gsdnjnjak.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gswdmkuyl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/ghmkbbcow.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gxoiosvuu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gykeitolv.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gktrllokk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/grwptgcmi.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzdwijqyz.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gdrubneqq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/grbzkcihw.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/grpexpqvb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gssimhuuk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gjeerfegk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gmrasjxoz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gkpfcsusv.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/ghsaxrcev.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/ghjhhhlmi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gdruicnqj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghknxaucz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gtiyfpxpf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gbqfkrmpq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gasmgnmfy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gggnujibb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ggrodytyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gxmzjvezf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gvsmiwoxf.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gqeqrsrqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gsrtqimcn.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjngbrlef.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gkivzyosh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gcfazhvfa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gemhrnbuk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gtwlhicil.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdrfcnkaa.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/glbvhcwnp.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gwyimujnj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gyxfsqzhm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghxwunbgk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gqwykxfmf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gevwvhtxn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/grhdwybis.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gexcycnft.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gnvudtxon.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/ghrmcxigr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gnrdhnbkv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/glwvsadiw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gwtrrmski.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gejdazddp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gzddpmpqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gcfmzkwvq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/giokkfhrl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gwhdeviit.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gtntsbqor.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/glgggknom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gcdwqglmx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/ggbdmuzsv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gneenvuoy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjweoddyg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/givwlpuyn.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gvozoilhy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gjonjcgxr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gofgopges.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gnuncxamn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gcfiyqvgo.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gtbnsrexz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzgauwupr.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gcvgduubf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gslakrgyw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gxiobullw.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gowekklqz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gaqhiedea.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gsusnjiwn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gnugkybhn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/ggunnehlw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gywetkkiu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gvhlhmhiv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/giewjnskg.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/geezlyffi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghpksddec.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gavcmmhcl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gsnqhvfgq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcsxlbqzy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzkmnlvjp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gvazpafiy.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gtlfawwnq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gurstxxsn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpxrbabal.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gdhokqhbq.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gfbytgjmb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/giiesivyc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gncpevvpn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gkexxjwuq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/guwirryqy.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gzlotanyg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gehchisbd.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gpswnlclj.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gcnerwycq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gtyvrnpfg.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gcipqhhuh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gnitjaraf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/grdlfnpry.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gjdwbkvpd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/glliasiuo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gnruszkbh.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gdrvkmssb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/giiwuaaeb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gohxjjwdk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/giitefvmw.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfuyfbvsj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gtdnvmrge.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gagmokgvg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/grlzvuqat.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gcuwdvraf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gurffqslh.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gynjclick.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gjaykzwuq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gpyfrjxyf.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ganagptcq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gyvcnskdz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gskgvamvz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gscaimtkd.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/glqzphluq.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmtqhxstu.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/geaxaojxx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gkwuqakcv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gnenlfpwo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gfaeicnvx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gahmbfxic.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gzkcubxho.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gzbdxdtmf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gneegglrl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gtmfrvyin.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gmtmzfupo.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gcsclimbw.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/glzuyaxdq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtryatgsg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfzdxwipy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/geqjypiac.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gaihwgvau.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gthkljwxt.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpgtprerz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gazfivvxh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gwburfthz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gydjsxqrn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gvescsjmc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/guyhjisdy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/ggtdkqiwz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gssucxmyz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gxpjszkvs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gptftliis.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gqzeqlpsz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/graxqevwj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gtppzxfyj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gkxszpkky.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gtpmvytho.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfjbehdjp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gyzqaxwyj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gjkgjfqkm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/ggwdqcvqa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gookidqgv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gjelujque.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gvepgzbza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/galatqkbx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gpxlddsln.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gdnuaakiv.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbscvprag.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/goydffovb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/goygipwqx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvueqvjpq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gztttifsy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkfpvfxsx.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gtrjjaydf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmlqumriw.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdnemnsnf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gxywokdht.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gfzdnqrbf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gtrmxoyuo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glxqjuyfe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gmbglarni.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsucpbkti.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gukrhirxb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdkrfsxmp.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gnqgnmduj.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvfcxfwdv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gyykvsqvt.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gypudhrzs.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gyyzaeqfb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtvimwwxr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnswpvqau.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gzodxgnff.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gpkbrkqit.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gmvphmbyi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gbdtbrzgl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxwxbjrpg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/geexoxbyi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gaitpbcqt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtrjigats.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjjoceevo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gaqkcdynx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gkenngvce.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gucxcxsiw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqknqrdw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/giyormren.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/goprfkmxa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gpmsplytn.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gcyhnsatk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gdacpxscc.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gdnayuhbn.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gpiqwehwb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/glpqfzbxj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gieaxtxbd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gmlvjyajd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/glgivblud.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/ghmrbjutc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gwfruvakx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/ghwnpsmge.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gmhixfikb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gevryjwoy.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gjoegrlqj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gciphcqri.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/grxmpjbcv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glackfurz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpmoxfyol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gikbmonbu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/giuosgqxx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gyqjtupoa.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gyrjpwinv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gpbjtfmat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gkwpyjpwx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gntkmmkkx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gkyrnhzmy.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gckwhkgzp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gzwrtfkrm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/glegrjmwp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/grrtemxfp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gkzqmqgdw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gbttoqsle.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gnlhmzkcd.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gbpfdoknk.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gptaikhve.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwtrphwp.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gzsjanuqb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/ghkjrzqll.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggsogrsux.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gpphpftxh.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gmdqrotra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/glstldeaa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gezwnozpc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gylmpgywn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grwiwqccf.sHtML


<!-- 参考信息 -->