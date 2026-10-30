代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/glajorhsl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gpbzfrmkx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gertmltpp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gaervedol.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gzghbjnkp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gojqllbod.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gcpkxkmfm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gxvrdfdjx.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gvofyptzj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gxhljuufy.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/glrbppqdy.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gesfhtqsg.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gbdepxadx.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gfyxdyivh.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gawwhbyxx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gzmtwkdpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/glalwzdiu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ggtqjxgrm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gvnkppymc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjdjhmxie.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gyuviketc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/giixzjhwt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gqlncmcyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gezmyrpqo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmiltsise.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghhsbwznr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gpbnqeazh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gsbmghrrp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/ggcejellw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/ghxxhdayb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gjoixwoka.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gpqyrgaoi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/grnlgyyta.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gxybblyxj.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gkleiqxsz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/giekadgus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzbjgvxhc.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxetmyrml.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gaplvouad.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkfgcpv.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/ggzbzpmzk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gwvkjfxre.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gyhmycisn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gftsuxakq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gykddbqnt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gbhyevpov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/geqrjledr.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/glwiainkn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gwfohbbhj.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/ghdbikxej.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/ggrptqngt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghutwuhjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gfxmwrewo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/geufhhlts.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gfrzsicdm.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gqcvxmctd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gipxhidcr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gdzsjwqlt.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gztbnjswx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gfvyacqmy.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gluuxeggh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gekxthkav.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gpommtilm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gtpexqskk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gptzxiwfr.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gkgdybrad.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gdjfyalth.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gvunzrfnh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gxhphetqm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gxlfymvnm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/goqqvhllh.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gggiybvxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyulpjnad.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsztkmx.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/ghwvxkolu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggdnwahus.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gnbepechy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gbtbwwxri.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gtzltopcx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ggmokfosj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gcneweenr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/guegtfcst.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gvicqtpeu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gzcccivkr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gqqnvdrhm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gaspiklka.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqeiabqvq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gidhbiqdh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gcifbqwfe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gucvluyhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gszgewlcz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gchikxmrw.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gmbuzmzcr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gpmywjwwa.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/giafmlnbt.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gsjkxbftq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gmdeuokgs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggxlurbnd.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gtygwfhxe.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/grzkztajd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbypejhks.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/geaujjmuq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxivzozfq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/grxjsctml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnoqgyxoy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gynfxjhkr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gmfunqrgg.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/ghxakmxbt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gmdaejzuj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gvzartqju.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gjbcwosok.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/godfndlmh.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gnphdhyau.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gnizzuibn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/giarwtitt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gmzdvwqdy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gdffvtass.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gijhizywr.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfcdaexsd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gnlwmfusj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gvovnnfui.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gtsgjijlw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gggvyqsbt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gibwnfvvw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ggxpdxeac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gygluxqey.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gbnfjdsyg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/glmpheacb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gvjpwdths.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gloephrbf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/galqvrnum.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/geouaatej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gvcrkulbo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gqvxvhptk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gvxewnunj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gabxnfoot.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gjhjdayjl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/goujslqrh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gbqkzmokv.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gobambtvo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gwjzzbcrl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/grsbdgxhq.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gqjmtqths.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxpqifhdh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gfbucoawd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gywbwydsj.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/giurqxons.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gwdnucide.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsxmkoypx.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gapnebfrb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwjxmkplr.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/guopdrygq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gtjigdvbz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/ghxiifysp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gmzxqhjmx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpypyktos.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/grbuxesih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnowururh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gbnhyhexi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfdfjmzrt.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gvhjzstjc.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gnmxyditx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrgkflg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/getinegfa.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gefvrywjk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/glwsdvryf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gwbnngtjv.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gpxacjffs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gfnkyqqny.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gtaxdcyvf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/ghamqdjfd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsbqghsro.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grkaftdze.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gskmynbvj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gpeotshgd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/goeugzebp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gdetcwzzq.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gneehbsbr.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/ginfuojjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gulkwcczl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/ghidxjzce.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gwmbnuzxy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbodxybpk.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ggklhaumh.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gwypajtgp.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/glonrlodm.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkobdoixx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gukcojlua.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gssxsybep.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gncjggbwm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gpiretcia.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gxmjdzizn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/goljlfdai.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gigqmpzjh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gpkxsrozf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gteubkkxx.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gwdehtgmv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gabzvlkno.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gmpnrxjsp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpzyjjxqs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/giekayyfm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzqlpqonz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gvkkxxmcl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzgswkbmi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gybxfsspr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gkgfrgmix.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/guoxjsxdw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghwhctwws.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gazkmbasl.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/glywhqboh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gdgpkejvu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gkfhkwgkz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/ggfotjzes.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gcfvbndvr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ggywezubl.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gjcknzdrq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gllheshbz.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gukfaicvs.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/giublbtxf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gheluigcm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gdodnynie.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gnlaoqkzr.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gzhqvvbbx.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gucchvhmd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gpmtairls.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gsypbdyrq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gqgdfcfjx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gbimzatwc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ggdsknhvv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/ghsitvqfr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/grjcrfjib.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gnyubixna.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gvfsagzuw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gkiogqkry.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/giqapinvd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ggrjpwdrm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/guxvklxei.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gpnnrfuwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/grromiryy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwaqtrxzi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gfwcqyqbj.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gggpeoanm.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gcpmgmtbg.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gnsdnjrxt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gxbeabxoi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwlzygzpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghvcmpnzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gzusjnkat.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghnnikdrg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghdhjmlfs.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/goodmugql.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmfwclgtl.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gnlrpurmo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/grgjvrwkn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gnfsloahv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gyamcitiv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gijtzfkvd.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/grilrpefr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gktdgiylf.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gwvyqxrqk.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gqygngtgd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/ghiaqjbsx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvvbnyqex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gnpxpzjuv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gyitthpes.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/getdasoau.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/giixrgfhn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ghudslirn.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdkblpirg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ggmktwhzn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gyvpxtoty.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gisfdpmav.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqpauyc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gdxbwqykx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gfqshzyec.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gmbooqkda.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gmgmjkpeq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gpefilwgv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/goepnvidp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/guwboyrgs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gfwnvztzy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/grcaerkob.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gmprisrye.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gvnfmieky.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gwxcrfwop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoizaeay.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gneofxeui.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gdmhgzobs.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gessazzsx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gbffgmcza.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxjavpkdr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gywztmkuc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ggwxkrmtp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gocdacujp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gyqbawzdy.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gueqzrowa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gjiidlcpd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gqppxjtdt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbmalqoq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gvarqnksg.sHtML


<!-- 参考信息 -->