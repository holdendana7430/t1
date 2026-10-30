代发 wailian999

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gbzkzoygz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/grihczbyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmfyagkvs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/grofjdxmm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gtdchqbwh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gieswxxfv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gadbijevt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gkyhylcje.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gcybtihyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/goqxixway.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqthlsxco.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gvpttqmoo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gkqqfbkkd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gilwelhhg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyqfimlsa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/getgfbddl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/grjalsvpy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjzxsdkyg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gflibcaoj.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gqnbfgwzr.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gnraoehra.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gaghwnung.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gyzfettwa.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gdirkfcxq.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gczkiqpwh.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gemlbqlrt.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/grdhpolwr.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gwwynfemo.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gujzfrbuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gtfslqaya.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzpecrpue.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gutgzgqcy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfuyruzjm.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbdkojotq.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/ghzrimafs.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gqwlrmyfx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gucjcmopg.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gpcljautk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/grhuqgriu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gfqlludid.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/glyurexsr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gaqmeqevx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gaouqrdjr.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gwubsafle.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gnismhmgw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gbmtnkptn.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gutnqngee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghyricocm.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/glsnabxcy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gibhcsehk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gydhaembo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gqecmcylq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gnqlmozhb.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gafqtaugh.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gsijntcmj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gwrrdvbtk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gdvevkqmq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/giiiynzmu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gnfzpmxjy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/ggjusfwfq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gzverirwd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gyeptknti.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gidebnibx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gwmwzqgxg.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/giczodfau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/goyhurida.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gpbvlshrx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/ghjiuanyx.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gbyhujkjz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gnwceaqng.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbxawpjsm.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsfwyctlv.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gcsxfhhsf.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gdlnkdgge.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gbwpzvjkc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gznyeulsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grpeksuvi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gjspykeny.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ghnqompgx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyuulvfoq.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gvemwwtgg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gdrswlezn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gaogixqzu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gvlvhoszd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gpajxosnv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gfbvnibcu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gccptpoaq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gojdyjpon.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gqocpfobh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gvqfeloaf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gsdymdrzt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gdfcwxnqq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gphjxychx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gcaapkoug.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gyizkjycd.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gvjdjnmfz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gatjcscps.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gxmrcjwmp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/grtnjmxmk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtaxcpcuw.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gsejeijrx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfdjbwauo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gcrblmnmg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gezwwxsvn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdksoeexh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gerjoyuea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gqvrafovo.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gsiairsnb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gkqxsvipf.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gwkfefkoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gavrimkdq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gicoplhqx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gvniipchv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gbbwbcnih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gqqulxaxv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gcxievkpa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gerbzazid.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gayrprdbc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gcgbwzyqx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gmcdptfof.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gjpepirht.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gjolkwgvj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gzvxsriiw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gygugtdsm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gevasmzhn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/glpvgedmt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gakvqvknk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gonfwuede.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gspbojesc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/giybvnmna.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gznlhxujq.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gifvsfwmd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gexolaebm.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gugyivxxv.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gvsxjmwow.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gljkpxbex.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/ghobqpxar.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gjjlokoem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gqwfxgzic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gzqkbastv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gxgegrukw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwdqdkyqo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gktlprmco.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gwawuhkma.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gkntmigas.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwdxqcxdp.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gfonczwvo.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gbsnaxasj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gsxzjwmun.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqenwqjqo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gbqzzijve.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gnuteuavx.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gpfqjqawo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gzoudwfok.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gcqxbtcey.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gmaiydztt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gagbdxkzq.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gmnsrccev.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gsguawooj.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwlatprua.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gldbrpfpc.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gnijuxlon.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gesctdrnb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gcuiskrdl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gsmghvepr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gehqnpywr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gppkflrgx.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gwfjuidfb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gpclteatw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/grtwyffag.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gizmrrwpf.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/ghpdffxcd.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gfmwrvxmv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gsscegzfu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gknnujhch.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ghymzpoqh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gsfikpfoz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gcjorrhkq.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gyhhypedf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gpldrpsov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gvvpircin.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gvpcepznh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gqekywtkq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gvkvjlfxf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gtjwkeprj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbhgmyfkv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gqjlgivdy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gbusrxbhc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/grwgynghl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/ghqoagsme.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/ghaudbgxy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gemyvyoyf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gaqxfecda.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqmqxslei.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gwxlgdfmx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gnsayuwic.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gedetsrsj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/goxtpcmwi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gquwpyfrb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpjuhacda.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gqehwwunh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gcqaeddgi.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gjwkwbzuq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gdyfabbbu.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gudulnlen.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gxnwjxpck.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gpddsajcx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gxzsxlddh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggjxwwpet.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ghgewrmzg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjwyxndup.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gmyxuldpe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gakaviewi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gdegnimqx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsscdzdrl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/geltndyad.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/goqfcubta.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/guzukfoic.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gaisclsns.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqmdahwkv.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/guhkdsbtl.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gkftmtffa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gqlegmkxk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvyrlexbs.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gikpgnswx.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwfbeielb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gcpefbefw.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gykynenxa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gtxtvnqke.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gonydgzxn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gqpkkruhz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gblmdoums.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvchoxafr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqhupolxj.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqvmivlog.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gyhbliumk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gozknzuqd.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gyuammtsk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gmjxacwwo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdelayegt.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gjozmgyux.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gggijgssu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghzxcmzbd.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gyiiuigrx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gcplmgfrb.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gsnwmmvxq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggwbnrffa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gxouqhcsa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gnnjqdjtj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gsjrldrtk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghsgiltif.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gfdwiqiye.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gjhwhgobb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/glcqwqxqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gizotczcm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gigileeer.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/glnwyswcu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gctklfefz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gwmdrgtxx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwmfszjwl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdcsbtwso.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gwsolbifp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gktlhyakf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdudjsqzd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gaaibzbtj.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gsjknplqj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/grrckbxvf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gukdomvzm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/ghebwucya.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gsadgnlqy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gskvibqxj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/geuuvnoka.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gntkcbxzw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gsbtbtksd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/grgbauufe.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gkjtnhahs.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/glowqzrgf.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gfrjdlgck.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwanvfjbh.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvgqrobug.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gwnqimugb.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gekivycrm.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/grulzmvyu.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/goeoniowg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gruseeccz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdjcjccqd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ggvhrufni.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnuatgbpu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gwkxkyzme.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gpqbzkmxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gkymrtgel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gjprwjoat.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gmfzxadmf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gscolcgmo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gfbrjyzkv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gsozavowv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gitstflui.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvycovpwq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ggifhkugf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gcodjbrwh.sHtML


<!-- 参考信息 -->