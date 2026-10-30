代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzgxgcntf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/golpoqomi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gersluhqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gxrufkssc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/ggelhlokb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gulitebvb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gzewcniuv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gimybukqh.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/grgubxqvs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/goghldzsr.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/ganlvnefp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gichbkggh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gzzmdepew.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gjpklknso.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gwvnybbis.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gfpyefoct.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gkkdxmmbd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfvofiy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/geyndedad.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/ggzgnzmww.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gieekfjvz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gvbfzwyaz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gamardpzv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggduqvxic.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gfdtilpuh.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gjhaetysx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gpkqkzgcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gullshkhj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gmuoqjxkq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gamwmzyew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjbazrmgu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gikbqdfip.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gwvfzlktg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gwinyimcw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gauopmpvv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gxylgplvx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gqyshlxif.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gviaaboma.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/galdetdrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gvcygczrb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gkffqrndz.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxufvfoxp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghiwnxbfr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/giafmfwhr.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/ggbggndio.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gfskjajbn.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gdinsejbu.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gtvdscjap.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gnjpxwunk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gnlneryoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gtrebekko.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gkkgxyyqs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzprlccta.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gcaihuqsd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzukufffz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gazhqcyba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ggyimnugh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gajgsxjnl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gzbqctodj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gohqqxuqs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gginvxhen.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/ggeldlfkz.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gnsyyrdso.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gpwouieaq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gvtsfpyfl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyikrksd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gbsgvgqbd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gibgofbun.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjdgmvwtx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gojmakdxa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gcgksixcw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gewscqnaf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gnlldnzty.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gzjewtzrs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gzsxonecd.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gajcqvfrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gmtxrshfj.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gnlnlsmkw.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gdytvkejd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/ghpgpegxr.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gvdokhqyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gqnzcjnem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gsaadvdfu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gwjyounnz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gmxjgqdjs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gjlzazzsl.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gnxclmbqy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gpviseotk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gsaxdxfux.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gymplavqm.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gajupzfcq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gpsydclih.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gcsturgdo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gaoolxokf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gdjbyrjpx.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gaiwpczmd.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gfltjnpjh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gapkylvep.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/guzfoehim.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/guuzhxtmk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gprnwyhtz.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmokyuzbf.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gkfflbakp.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwxrvlezl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjqbhuvav.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gulkffyny.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/givonpifr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtlmhdgys.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gqlomrkkl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gdpmotdkp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gbjcolvvo.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gwfmlydky.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/grmgntlwu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gnwuvobnl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/giajrmaoo.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gzjxsyxaw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/glqjkjvht.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gudvalqvz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gowsvuoew.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gslievkok.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkhekolfj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gurxhcqrd.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzqoxgvuf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gjklhzwrl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gorctfuvs.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/glqrkvarr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggeavfdqe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gvyidujmu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gqdszvejd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnuifegoy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gobfsixem.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gyqnttgtx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gkgoifoqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/ghqkapdfk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gnlxtuejm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gcqdzhnek.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gnxiyuffl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/ganpzbnll.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gojdvuoqw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gkdumgicy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gsfaibguj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/glpmsonlf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/geqqeyque.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmgffutaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/glpmfwpvh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/grrdcvliz.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtdrckwpd.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ggnfulcxy.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkeswvjdq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/goqkwhhgy.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcupbgbaf.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gsoggcmut.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gekoacijk.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gzdwwfxki.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpqutyiou.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyqhiigmg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gbjcnrefy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gtgouizce.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/ggzyevldh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gmdarrjmv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gsgqdmttg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjashhki.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gudeeuqvm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gscwfnwxp.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gisepwxia.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/guphdnbct.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gplqrjggv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gcyongjnk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gslwgpxqe.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtntqntpw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gzruyfoxx.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gfkapytsh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gwudiolim.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gnedsaosf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gshjwvcmo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gsaikudfv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gddajgitq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvljcobhr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gdhjaforj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmkueefmj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gvnpgnpnk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gwbemodco.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gdcforxgs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gkniyhkbc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gycbqfvro.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/goduyohfx.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gegnpakki.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gdklnamdy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gwvodblos.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/geesagovj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gkzuldacy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gfpqayexk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gdfsfcpgt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gtglgcmec.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gvmfghyur.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gmrlbnacm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdjxnokns.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/geghstzdt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ghkhahqbd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gngupoiak.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/guvnpqydw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gzdqttlkl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gmaxzelkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghpogzaow.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjxfjgzvv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gphnbvhon.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gbvbfshaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqxspustu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggoptlcth.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gyyiwmnwj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gkhlfwziv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gwfuyqhkh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gnymlcjfa.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gumzhrfvr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gjwdzftnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gqerqzgkl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gfwmebzyp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gffkecoaf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gziizemmz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkpgsyl.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/grmujuvef.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/grttdtwge.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsvokgacx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmdlbwjuw.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/glzjabmqo.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/glbbxkcre.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/giklphngb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gdsbvvtqb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gispbhkgo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gqflpvazm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmjarcmwo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gnxaoeglu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gwrxvdhya.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gtfqfvlcz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gtczirfju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gfmueqchm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gfnovltzs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghyibjbrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gzoilkhat.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grgmofxgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gspwbijbg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnvvthdsj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gaxvfuvyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmsykqdtt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gmgxwstxk.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ggktchnqi.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gmyiqauhj.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtztkizvn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/guffzrjxy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goblpwjzb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gfpnbnhhq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuygztr.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/ggcirnufp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gyarkbwbt.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gvetjaovi.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gjrtsecux.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/ghjwghwnf.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gubqlyebj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gpbpuncnx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gnpvosyjc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ggxymjdfy.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gwlcccoqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gahhyuuqi.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gvvlnjwwo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gkpeluath.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gozffrzks.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/guwvitoic.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gphciuesa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/ggsrigkin.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gzpzwiqjq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gmcjwnrta.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdqfdmlfm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gnhgwjkvl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gxnqhyokr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gfeufgbrc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gsvoyccxz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gfzjwrdto.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/grixfktos.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gvhohxfen.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gwacctigu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcmhugovg.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gqpuzdowb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/ggaivawdf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gjwkbtcvf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gzutfphpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gdnlfiqji.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gbyjayldk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/giqxygkti.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gejdcshsf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gspnmafmz.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gnwwlcgjc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gnkfzzfhw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gqayjycpo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/glzipfphh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/glxqszfvt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/glfjoxwwi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gdasxvqof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gwnghzyjz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/guqdakbjs.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdrpzvc.sHtML


<!-- 参考信息 -->