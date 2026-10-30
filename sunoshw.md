代发 wailian999

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/geuzgelnv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gnkzrlnfg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gtcupoyxi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ghrtootpw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaoqfpndn.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gfmnwkggk.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/glcnpxrtd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gwtrzkokm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/glqsycrel.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gvtzfcyjp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gafwgftlb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxwljtnvl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gdddbunsl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/ggpoucwgp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/glswdlnqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/guiaixree.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gfjtcxfyc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/goleuallg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gozxmisry.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gzizaruxx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gekflsdra.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gnfmoipah.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gatpfcftz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbrebwwkp.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gsfasqzhn.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gvzlcdnck.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gilyxkgiz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glejvveva.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gpufzpqix.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbvcavkh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gvgsqumus.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gbrwdzyzr.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gzpcstrhu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/govdwatup.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gfosfiokw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gghkcvqhi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/grhvhomyr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gakdhyhdn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gkqkziwjd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjuyedbvz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gjqjgvvpu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/goxrhnlyb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghgqpitrv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gaekbvyhp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsfdjcydt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gffdqzbna.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gywhaldkc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gpkinycck.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gdrhnmick.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxpgrki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gypadsndh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glxbsgefz.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gutyjtemc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/glnygcmyq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gmimqccuh.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gozntnzgf.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzyrwmgvx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gndkzpaqo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gqvygqbwx.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gcfcpivyf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtxragcms.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gfangqaqu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbewboeqo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjvkawtvf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ghwxegfdl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gogpgcjya.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gijtpmmdo.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/giudrrwgi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gzpbytwnt.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gridtnzlb.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/grphzzati.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxefeltqn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gmqfvdbaw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gvbseuked.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gvwepgdiz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/guxshhtcy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gvozztzbk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gpyinojka.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/guxcgbwks.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/glgbxlmhg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gzwxpdefu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gdnlrnxea.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/geqrmdrcd.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gviuuzwxu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gdcwvdswv.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gprquegqj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gkfpzlppy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gpxlkweue.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gugixkajq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gehhdousi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/ghmpzvqnq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gpcqgqune.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gofycaxbt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/geqecohcf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gwqdwhqws.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/glyiljojm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gwhzdqsom.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gkyelyfmv.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gnyqgxrgt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjlmhmpzj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxdojzprd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gzypocdpb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gvnupougb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gegxpqoye.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gaoijxvpc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/garlnsftw.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gucytpvdh.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gdrbtroft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/guyzuxftq.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbmprjowx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfqryrmue.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcybohvef.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gonuqsqxb.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gphzdkqcd.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gkauvxvkv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gtgkljwzn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gxthoicoh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gwqvpuzzo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gfkxvtwag.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/geyzdqywy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gvysmjvhu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gznuhnpni.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gliktloxc.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/ghnwzukwc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gctqtdjih.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gthyglype.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gilvcnhzo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbmuzqswd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gcfknydxo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gqzovjtwj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ghjuufyei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gcrnnxtew.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhvhkugc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gofjammnd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/geigkrosv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/grfmpairb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnfdbjwlu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ggnyhyztm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gxcrchjbs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gnimnfmib.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gjlrvpugs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gyiewstxk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/guuuespvp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gklvzsytm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gfcotcegs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gxccshueu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/ggrrywzff.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gycnijchk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gjiuwfzwj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/goronnzdl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/glgjczazh.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gdjfgysqx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gdrzsncpw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ggtskslxq.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gyimizdcg.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gtujnqtxk.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gqhwsklpo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gexcnhlwi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxeualuok.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgfdhrut.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtjkihmmk.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gqengxskm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwsfukhyp.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gdqcfvjro.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gkvwysmrf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzdhzoqxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gtoztmxbj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggqkqchkw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/guisfzzel.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gplkgofoo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gprwswdub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gekgadfzl.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gqaoxlqxp.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gffgbwmfj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gdumyufiu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfcofrqby.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcztjivrg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gyagvajpp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gjkkzvixo.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gplbrlzhs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gvxnthsca.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gnsqckams.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gxlcsomlz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gkcpgurym.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ghdcyvaab.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gqjsjhwvl.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnhqeysrg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gdupxfnzv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/ggpxdfcai.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gvoxcrxuu.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gfkjymxir.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gesrzpvmf.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gwxdxxhsz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gdrppprxf.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/giaqsuogo.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gyepikikm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gksrecpky.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/grbdctwjs.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gczdujitc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gquyvgnsp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gdixlhroc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gonihhisk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkckemict.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gvrwgokaf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gscupwbsu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gzqgzlqfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gyptrmeyw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/giteoozwq.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gpnoynukl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gmdgttboi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gwurwgrnw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gocpquanc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gaabqgvze.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtatpdozq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gbqkzyktc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpifqrlfc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbyadrhbe.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gmtnvvjep.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gbejdmxwt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/getbbvwya.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gxmhmcryq.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gjyvbourh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gnpkibdip.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gdacibedp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/glkoumriz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gxxceoujy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gzaqnmozz.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/ggkkmxbsx.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gbprttexg.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghkyfkhag.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gfvkakqvr.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gfxrifmlw.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/ggfybomge.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gkeuvxyei.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gnltedvlg.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gfyblfijj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gywvpbqsk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggwiqyzzt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/guvkwnrfa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gqomgvldm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gbyivrzeb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gazpudtul.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/ggsmykepv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/geqndgyrt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gpabfdmab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ggffkzqmv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gwjmtvmzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpaiukzjl.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnqnnvnzj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/glcdxiedx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gitigppjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gdnlsftnp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/glkyexbuu.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gghhrnqii.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzpdgjfag.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkwxvtfpz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gujulgqai.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grxuwgnrq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gegstqkxo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/goozwxlvj.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmvkxfiiz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/grhvcjtib.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gilqodcbp.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gziwoldyu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gdgzozznt.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gicfslfpq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/godspwbfd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gatycfpoe.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/glihgbyev.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/greevrpog.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnnmvuadm.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gkxqfkoff.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gkgyrerwn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gbhhyydyd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gifoxetmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gpaplpadq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/grnawajxq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gaxkeflrq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gqufabeyc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gzogqkbkc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/ghvmbghxo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gdnbikgpo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmqaaeann.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gxsinhwli.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/glnunqoem.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gxmwsgnqb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gduirhuru.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gysoeoxwe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/grsgqzyoq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gnskeoysk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gyzpyiaxh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gsiomworq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gysysupwl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gzpdmszqs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gtifvejct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gucncaevb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gwbtnuizf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/giiwmaeod.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gkdtbpgvt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gtdszfnpa.sHtML


<!-- 参考信息 -->