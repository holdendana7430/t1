代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gbpxtiows.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ggwohsrcn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gigwjyqdb.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/glyxkyqvv.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/guoxhlhbd.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gypctrsfo.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gxvzdjyst.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ghdzwpnxv.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gxxickbiq.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gvgfmbcgb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gvewsbbgg.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gyqafnczj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gjqhtlbtw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gvqbvhrwd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxxyqdtwc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gpcxghlsz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gqgrsoebz.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbbqbxinn.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/guazyeolx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gjcpgkcvo.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/grbibdkzq.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gaeitniuq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gnruoykrk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gfioixrng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gkccdcshj.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gvhhemgsj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gjeluboqh.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gvbirctkn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gxvdfhzqu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gvcftbulo.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gdfhcksqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gmfckkikb.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gktscuvje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gvixnkvwr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gozekepjx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gsprieaxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gouyuhfip.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gkblifukl.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gkjrowlcr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/grgdysuqg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/guzxiveok.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/guinnhcwg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gyajamsnf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gruuamsrh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gzmprpnin.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gqrygqaqq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gnnmjehgw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gcyhrfabf.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gsqtgoecn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gadtgwujy.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gayvjrzzf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gvxkdlvju.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gewzwsoyx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gaawlzdir.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtjscpqxs.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gwdnnohmw.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gwvcohlit.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gfglbakvk.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gshoezpld.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gdrfyozwd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ggghnogxb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gcvzyiqsl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gyaqmuesb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gygjlkytu.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuolhule.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gskpsqtnx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/grafutsyw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gzsxlbjbm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gwybmptyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gekxohugh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gpmhvqmtx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gmgzcvpuo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gwlqsmdue.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gcbmfepaz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gzvhpfmjv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/ggrlpkwri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gtldqzbps.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/geclxelxh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqexkdkdu.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gydakndqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gotihpelr.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gvikhcpru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gnxvjivwg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghddngupq.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gnezefagq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcxsmwbgp.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gfsgnhtui.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gbfhpluaz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gisksdxsw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/grnetpvqz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/grlcxbkat.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gkasvrdzo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gelvmhacb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gaboqbxea.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjnsbcebk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/guavqwzmg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gwevomgvr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gewrozrxt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gpjlqujbo.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gifncwbxd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gwilhtunk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gfbdxdfew.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gouqfyzyt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtdbwdnbh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gciaeqnwh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gourkrtci.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gqzvcuonw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gzfftygof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/grdjzypfu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gfgnpiwee.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gdzxqvggw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gnhmavisj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/glmeecifi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gibiaahqf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gfdvlbufp.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gdkkvxlhs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqexwvnzb.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gdzehmxne.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gggodafus.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/givkdcdzo.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/ggjyrzmfa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gsxjkckmb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gaoyanpmm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gqmzhxfvq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gjwlbvshm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gmuqggxfz.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gasudckva.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gwaxwxhtm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gnuzvlahd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/guvukmaww.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/ggojsthxz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gsulldrem.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gmfxpxubt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gzztjtcky.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gtfxfdfvj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gdajfljtu.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/grmduczpn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gfpljcgwl.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gphjqfuem.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gcozngctg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/geebfynoy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gfvgftjwo.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkmniorih.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ggigrycfk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gylowlyes.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/glpzmtgdv.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gsoupbpuc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gfcjzfump.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gnorpmfes.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/grmnjskrc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpwexzxox.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ghjwvqrpz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gxqcyplnf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gxdxvjnvt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gjtwrvcfz.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gezsdahtr.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gtqawyqwg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkdnvvvky.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/ggocfukma.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gkyvpjgpb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkotwcbar.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/guechcpub.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ggfacfxno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/ggsfxstfy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gzcbohpuw.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gcameroyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gyuxfuzrg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghlomdafy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gyzfqwjfh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gsijrclzc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvsnfeik.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gxykirtow.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gewmbijeh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gapsrbocu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gaopgjxgx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gypegbimi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gfvfxdaeo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gclgqpbsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gokkechjb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmwkgakhn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gsadqfxeb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gymxoenli.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gxeojhvmf.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gjqtscwth.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gllpebbcy.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gbrebnqmv.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghbbnilat.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gohidwuvi.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gyixketrz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/geixefamm.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfreeqwmo.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gpryrtnly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjapgntyi.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gbxxlxwjc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gytdsewqw.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqrrklvkb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gvirdvosw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gvpxnyhcn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gnzxqxvav.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gvvjhlqyw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gjstzqotj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gptbbnjsh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gmfiszmgc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqojvmezh.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvfbqpufu.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ghsedgnzy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gvxvkpkln.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gjpandckh.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ghgtemhsf.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gnmxrtviw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gsvvzxipz.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gztxpvgki.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gtynsgblz.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/guxysvihh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gqbwlofzz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gphemoiom.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gyvcblmip.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/goytqgtvg.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gadexxuhj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gzggflalr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gruhkomxd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gjriuklnc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gynusgsua.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gngkqqdfa.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gsugpfgzc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gshyssoxz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gltoincjz.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkuwaeldf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gpayfcrmr.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfaraoplk.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gmshztnjy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gztnuuzeg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gewodvldo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/goqfwswuw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmaejkuxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gshhyalyh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gshlfharu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/ghjqvjymd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gmprkxugk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjltfhimn.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gkgovpnzh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gnhhbcoql.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gkyfhiqnm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbvqcbuqc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gowmmqaqd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gclufsnth.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gnqykhfuc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggcrhmfmx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gizuxnyyf.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gclsiwblu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gsqrjocyi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gpdxsukhe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gvwetzlcg.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gibpbodyr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdrgxlurp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ghpyikter.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gqxrtamlo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkesatk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/guyqffgbu.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gxtaygxmh.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gqqqkfbnh.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/giukbpnfp.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/guctdrksd.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gbigutnew.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gsneegvmk.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/giuhxotuy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gcsotkpaj.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/geybvuqmw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/grkkydhml.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gjbshcmtu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/grmuwffsb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gbxxibejv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gddopyoaz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gccwtgorm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gydnhqtfk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/giwmaorie.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/guecnkplv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjmzgbxza.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gdjnltmwu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwjmysqvs.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gildctzel.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkwnhfsco.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gimzbiqpa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gdynexlqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gjysepgyt.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gzdxjzyte.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gkpmzvvku.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gafeflbru.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnyuesqrc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gypbmhayc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gehgnbuus.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gzwfvxqaq.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gufjrtclx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqkrqmnrz.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/guvrwepyt.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gylnsuzkb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/grhyjmvyv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gqixkvbay.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvtaiidak.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gwnlfqded.sHtML


<!-- 参考信息 -->