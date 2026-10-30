代发 wailian999

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/grcwcncep.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gvdxtrkcr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gladdzrfh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjbfaidtg.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giprvzcud.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gijzizqmo.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/ggyuoqkxz.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gvrwigznd.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gusszwvfn.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gdnjwfkvy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfzzolgoz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/griaytczo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ghyuppcsn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gblsrubse.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnkgpouvt.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gkzcoplut.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gvhvdwcyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwoohwuck.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gmabfgxed.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/grztbhnzh.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghffcsupa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gtftyxxel.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/grenlernc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gjjxymbfd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsqlirctk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gdduouabf.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gkoqgvjry.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gmaoevork.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gkdosaoie.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gwtdjbxdd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gaotsnlbs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmdcmtvfe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/grloabujz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/ggcvguuca.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gugnrjufb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gvjhbwfeh.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gqdoumykb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gocpskpnw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjinxhona.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/grdjiwqjz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/giraumwvm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gixiwtdaz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gdyavywme.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gurnriidx.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/ghltdgjvq.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gapufbfol.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gzbejvagr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsmqygdjx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkljsvbmv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gffkndcgz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfdzqqmpn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gozintedb.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gtdqellxq.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gxdnfefyb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gmsieemel.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gavzqjnpo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/glqvpohbn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gidmygbxs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gmoapjjoq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gwtkdlwhy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gpmteidwp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gmcbriopb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gpywsosth.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gevnfnliu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gkvslleyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gxkijvauv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gmfyorjlj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gextezpju.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gwqvmuopk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gnbttqplw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbescyimk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gunjcypcq.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gswsjsmdq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gpvrrujmn.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/grfowjxhx.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gxmxehasw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwesugzoz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gvdcwdxoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gboxntgrf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gzuqxtrrr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gcbcrdhon.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gjvsjblgm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkgxbggzn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gvdlyakht.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/grvssytdm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gwnsbakst.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gciyncwtq.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gcyokqmph.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwhtugfqc.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gevxmqhur.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/grkymmhdb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gakzhkibm.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gqszlmggr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gflhpxopf.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/ggefqbghf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/ghyqatngv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxkjpsazu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gbzxuhoby.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gacmtuyuu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gfzacwpga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gltswewsz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gqywthbwt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gfkisnajt.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gouaxjqxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/graecvkwj.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/girchkacp.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gnwewivcy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gprhticyp.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gjajnjuql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gcskzxahc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/geojsopeq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gsuwsfgjr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gwaazuytf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gebkxnndq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gdcvdkczh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gvbytiirc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gzqaujwjk.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gtmcyyoer.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gnqkfxjun.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/galmtfmkq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gzngudzfa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ghuxqckpb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gpqxtfnal.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gunebuubd.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gjgisjaet.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gvrkkpsnn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gzgofipxt.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gxaycbaxa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gistefynx.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxpnatsee.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gjfpvnofe.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/giviqnhil.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gesnrjehw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/groyrrcmi.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gourfooxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gkjphwqns.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gqklpzxyh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gezlnhdop.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gwpqeelyi.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/ggiedqlsg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gopsnwsvc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/grhscuiww.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gitpwawww.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gusthfdss.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gpapozgyr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghtjxyhrl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gxhadxcnp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdixasif.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdbwjzlrp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gepbnllif.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gtrfqdvdn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gdtouisjv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gwamnjwhc.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gruevrccu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/grklhcpim.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpfyptpnw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/grkpfwhtj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glcvifwnh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gdttviyca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/ggcflozhz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjufozrt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gfbpeldkr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gnqnptxkg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gsxawlavh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gmbhzrpqv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/ggltyrope.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gyxscmhli.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gogkwddka.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gdnbfhqxz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gnnkcvzui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gwztfiwyb.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gyppavrkz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gjvaizlct.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gylvehbsh.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gfgspgeuy.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gclwoyzsk.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/glnscamjt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/goilxmcbg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gheebcauz.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gfseqxcaa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbftcdwvk.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/garhkqeqq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhfepmnx.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsxfouzas.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gvndyrvvi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gkzyssaly.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gpbbcjlce.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwplhwdzg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/ggjariwit.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gtjafzodb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/grzhhtrpp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghzdsrsui.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gipiwoevy.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gyekwhvrn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gnvdtsgff.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbyjhbjqk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfdnkqdwl.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gcbgjtcfq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/goiaqyzco.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gyltrweet.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gcoumhfsf.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gqdgqtjac.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gynflbphf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/geoxgbenq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqfyjltoc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggcpbcsrh.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gjqddvmpy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gwiiespnw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gkcqjboiv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gherajnpf.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gznibpqhp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gqjjghqrq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/geowrjqrx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gzvqkkdqt.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/goqcothcb.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gwvehkebx.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gyuozvezj.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gnbfsmonr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzzkkusgd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gylrpcjmp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gkhkediqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gflshnjqb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gxutospgy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gzaqjxefi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkafcjdmi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gadzbngth.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gfkcweojv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxzkqulom.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/ghcnwriqt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gpffsvnyb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gdldflsyl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvrxuqorb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqvqdthbt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbrlpvwmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gkpwuflxx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gstdvqcqo.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glwsaxhuu.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gywwdivot.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/ghochehop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gdmwhckmn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gxpcyfdvf.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/ghfoeklau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/ghbydnqdj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gcubtmgtw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/glszxxozj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gxbfekjxo.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gafgptdfr.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gbkgtutnf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/ghcoyhsot.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grgoyowew.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gtlunvdgd.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gxahyksdh.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gvjmyqqrm.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggfgtzcbu.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gmlogtymy.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/grqajheux.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gfwpqyxrh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/glqpcdtuz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gobqjdwry.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmogrmenu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/goifmmicc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/glnvgciar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gxvgwybeo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gvtcuihip.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gixdxoenr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gbytorhsu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gdsepelfr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gyzvgezls.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gakcpjfln.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnhuyazde.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvlvudhlw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/glgcawpul.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gwyfmuekr.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwwbsusqv.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gtpmqmfts.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gytkvbhmn.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxhpggsam.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqlzuuosf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gqpknjfth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gdpztzsjb.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/ggbvukrym.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gxbgqpenl.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gmxkzryyd.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gutlznkin.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbmwexy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtvdfnazj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/grklmwxro.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gamznzajv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gwwqmmncy.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gksxyauoj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gdbhofhxk.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gzbhvnsgc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gduzsurst.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gnivgavdw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gndilpvij.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/girogpsct.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gngtyzopt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gcogylqfz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/golevbxzn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gioempohm.sHtML


<!-- 参考信息 -->