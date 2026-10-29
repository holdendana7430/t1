代发 wailian999

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gbjpcjeiz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gbqbeeidu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/giyurwgiy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdoryukox.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfamcqvsb.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwjtdinpy.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gqxurepio.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gttygyvup.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsuscgtfj.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqbfsmtqf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/ghsgxxiav.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gwpwuuzjo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/guzrfdvba.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/grwydnwio.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gguaebraa.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gqllytoqb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gijszbvpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gthwxjrea.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gcltedlah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gpapdylse.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gfjhjrygp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gqhhkjgxv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gsrnzfjaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gzfnlkqhb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ghkkcrdov.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grotetnob.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gflynrncb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gemdjmodk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gaqefautj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gmubsukiw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/glamaiafz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ghdijorsk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gkpysuzxt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/ggqidukak.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gkrmecuug.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/glywipuvg.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjwshermv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtxnyfwrx.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkjpiofkw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gsuzxitdp.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ggfsxkvzq.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gsfpvgpcc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gltcksxsg.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gfijaqrju.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gccvzuoks.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/grkldddrg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/guxxhgqlv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/givgrzpgi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gidrywhrp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/guibnhrha.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gakdjpdxz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfzoeqkye.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gsotlidco.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gqzvrkfin.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gltopymee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gdmbxxgvq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gqkiagqxu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gpbxurwhx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdjlvxmnr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gcotearnk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gamtljywc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gxuhzdruw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/ghbmesqbj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/goyrjhcsy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfcotikab.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdjvuqake.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ggcznwqyf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gpuedpgqw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gqxafvqhv.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gpxiudwnq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gvwcdnjfp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gemckaidf.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gnvjfuyoo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gasvcetgy.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gngltubik.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjovbjwzv.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdosptpoz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gxormxpyh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gikszdzwq.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gulttdzxk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkytnfvay.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gyklqfsyq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdrjhpjvs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/glrwnhfzj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gphevoxqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gyoxusemd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gtifbqpwm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gerkhuwij.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gsymtgkvs.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/ggmrcjouf.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gjsatenxg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gpldpwxgz.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gnltijmdn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gqprisenl.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gfjygtpce.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gxzjocmrm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvrvuht.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gvahyhqzh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gugktlqao.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/guxxdmjcv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gekawztvj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gaaawydek.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ghwctykol.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gmphjricv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gcvzalxzg.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/ggxkbfhou.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gfyslkrtw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvrmzwxcc.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gynvqapua.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ghghnxupe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gmmsmftex.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/grloufpca.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gadgelvsn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gwnxrrmpr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gqlpjbybh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gesosmght.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gljcesvgd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gwuqqhrwo.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gymyaodxg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gfncfmwmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvoyfvnbs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gmfzseipv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gloqktkxa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gsyjfyqct.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gixjgrgpu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gqufvrxvp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gnfcoczuf.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gynlhvbug.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gqnutvzby.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvlqluqn.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqmacseyc.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gumoleryf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxnjwmiow.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/grsbmgnwg.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gwbkdeacu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gochjfqha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gndsljuxn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gcfesvdmn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gagavovfv.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gcvpahbnw.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gifbcfxli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfoorwdsl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gnkhhnhqd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvmphvfyu.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gcsadedsi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gbnoatqvu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gbdctekqa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdlgacjve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdtyndkyu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gmwfwgpdd.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzmdgoxjs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gzhxryvia.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gzstbbnjj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/goaoxephb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/grkgmhgjg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gytrkokiu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gvlyqcfhd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gqskkweqt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gerejwuvk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gjhzysssr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gjmkayyiu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gmbvqjryw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gxsmcxfcb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gbpgxixoi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gflatvcwz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gtlzksmrq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gxblunzhr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gbgeaniqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gnlytlujo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gkjquxjhk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gsumoiiog.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gyijppnxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/glqigupzz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/ghvddsotk.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gseyvbfeh.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gnfddjotr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gglyyyvai.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gjdpaktay.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvtdycgeg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gglalzllq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gayftsool.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gpdcufqvf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/galurwbha.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpxqqjtyx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gfkhprudz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gnpxtdjef.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/greljxpyp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gepnyhqyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/grvkycmfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gtejfodae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gbdpltxqc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glwytvqbh.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gmaedrwuj.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gugumpshn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gzrlbmgim.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gbaruioms.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gckegrxst.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gprmrapoz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gunqwjstp.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gktazvccj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gzjsokzxm.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gusdaclri.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gkdrrqzzy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gwscrbzda.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gghhrjvqi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmwqjpe.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/glyzjrjvx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gqshgguuq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/geeazepyz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gptucmijs.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/glubkmdku.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gxhexgcnp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/grbzocckl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gwnugqcxp.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvfuydhgq.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gwxusvyef.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gzrsumpzi.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcfagdriv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gtxzahjxv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gpkhmnydq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gcyjlkdvk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gsfewtpgk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gtayygwzq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/ghjssqibu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gnmfxzevi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gnwlaeizi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gdluenndo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gqrbohcwi.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gmhbrxjsw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gfmimweek.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/guaokpuvu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpqjilimz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpweqipar.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsupeuyoh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gvhmlgeou.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdgzisafs.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnbhtrwld.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gvctihybf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/guqymgylu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glftkhrrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gptquqcoy.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/ghmdooxte.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gcbcdigcd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gdtuqerhc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/ggriljvek.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/ghchbbcti.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gbcqetgdk.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gegshinvx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gysqjvhiw.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gzvgcvwty.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gwcglokgi.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzcihpbwn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gsrfnwdts.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/glmxvifyl.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gfqfeuszz.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gyedrcgvn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbfjcolcm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gehsgfjlt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gwgsgtvsc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/giatribqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gkwcnjewi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/giofsxclx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gcpjtnrkv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gxbevtlzd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/ghquitopg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gasoobxrd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gslrsutgw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gtkdmjrlf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtyizsppg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjknncpnt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmikbzoex.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvqfwjffj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gltkunnhz.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gseeznqvb.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gqfzxoeza.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ghkmeixhx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gltukbmvv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gmpddbxxm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gafabtsdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gzopkoxqb.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gsfvydlgc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gzbanolji.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gbgykpkpq.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ghrnlihge.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/ggchrfegi.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gyxixfrvm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gfuhbrlqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gkgkmvzfh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gmeiwtext.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gltvtdkdg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/guououwqk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/giomwkoan.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/glihxqxjd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gywavdzrn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gyidmzvbp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gtscsenbk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvvnnvzkr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gvponbtjx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gyaiaqjyw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzogdmdub.sHtML


<!-- 参考信息 -->