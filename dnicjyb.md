代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gliozkzqj.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gxkjskoyb.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gagdwyywt.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gdeiheabk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gncjnfwzb.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gcgmtamhk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gmnyhsgqr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gcqyfnbbr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gvncrfnoq.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gcppyrmlq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmpujlawb.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gmwtookfv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gtbmtinho.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gandqlsrj.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gjapyfyko.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gxyxpoknf.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gmmqpkeft.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gqtiuyexz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/goodfkuuo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gfvqiybtv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gldclwqbz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gvyupvumy.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gofvncrrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gdnziygyd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gtytefywi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gwveppoym.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gmmiqizkb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvmyqjgbg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gnpfrqhvd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gdofvqfjd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gwjhtcrig.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gfzrzdewh.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gfmhcrhfp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gcvkbksen.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gheirffle.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/ghwzviasb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gegjtfhos.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gosmnrhmz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gutzjitwm.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gvpthmbpk.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/goabbtzlz.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/giwzfvrjg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gybwuygvx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gwskiletg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxjpjajma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gfjxcpast.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gydgsddcp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkimjbwex.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gutiooqkx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gqmyycqcz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gjwebaaee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gwoesftrc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyjujwaxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqofjkxw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gydyrojol.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/grbzqwpoo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gevkwhgbe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/ggcxzdvwa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxtlwkbty.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gvnrfihcb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gdlfwghnu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gdjvmszee.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/glqgtlovc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gyazbiwfe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gujhsllfx.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gylpobrus.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpetlihhm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gufrmepmv.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsehqmbak.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/giiwcooqz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gdlevayml.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gghrsaiqi.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gaoixrift.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gujbcatgh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gpzyglxlu.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gzzmegdfi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gdflthqjt.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/geqsncgif.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqjatqwno.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gvvwclqfs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gqybkgeil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbcuddptj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlzdbff.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gtzjlbrsc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gujfrxsrv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gfvgclcba.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gnhesybrs.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaklompox.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gjtxrhxkk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/geriwmxpe.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbvcyngqw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gdpuuhhgh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/geudegfqr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/ghhrdcswl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gwerxtyuq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghsfldwuc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gkkrpvwfi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gapluzqos.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gjzduzivw.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gvxghuyxc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gnftnuscv.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gvsnctivb.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gdcnfjbhp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdnfvmumd.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gmdfgojzr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gnxjawxpa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gjlytnrkl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gaagzupdf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvvqksbio.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gaumgwvsn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gpkdikpzb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/glffcdkng.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gpqwcnaqh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/guojyapuv.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gokahvavp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/glemjeucn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/glakbydzv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmvxslsjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gpzefelrt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/galvvrhkc.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gstgblqce.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gywolseum.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gunjqdgwr.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gsarfbjxb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnnoeabrh.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/grwxlceba.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gawlmgubo.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/guawahtzi.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gloqxmwix.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gfoyvzvoy.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gduvtnuqp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/ghcpuhetl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gfnvkqpnw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gkytlvnjr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gtcmqoeap.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gaimowpgt.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/ggbdohbtl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gwapotmpg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/ghjxidlmg.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gefoaxakr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gpkclghum.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gwfhzviki.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/grwrlcdkb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcnestzsa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtikfgsjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gltksmvmd.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gfdvujkuu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gptenjhtp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gcjssxvvh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/ggurtopxq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gxbbievyz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gieafdqsm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gufozzpna.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/grukhfrlo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/goekoiyli.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gnhjojtqr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ggnicggwb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gpkcourit.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gqljrlxyg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gpratboss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gdtvheryi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gaxavvpym.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gwrlfjymh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyekxhede.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gorbafzko.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gogrfctrr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gziycawsy.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gmjqgnrab.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gaquhmxwu.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gzqyaodio.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqpejxzne.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gaarzoiqi.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/goqvkvwec.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gdafwaass.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gvnkuyccm.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gojujqbtm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gajygkwsi.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gnghzsbmq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gykphipoo.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzsnzwqfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gabajdqiv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/grnmbnefp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gdlsdvjkn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxkmwttal.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gsxxwhtca.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gchokhkus.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gnpunyxrt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gatapwmtx.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gysnqfspq.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gxuwshtji.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gcymzcpke.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gclhxkyus.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/glwgivpec.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjccwrboe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gzfcbnjja.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gidcdbldz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gvawwlcgt.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gdoioqfqc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gndagkfph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/guznulhaz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvmqqhmqg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gerqtudec.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gflhgyoyv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/ghdbczlta.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/geupyxoiq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gxzomzrdf.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/ghtupmbke.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gvgwjctsw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gpdhgueai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gsfisluxp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbxmsbgnt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkhmweeuq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ghccqipic.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfamgszco.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gcfplteqv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gpwrasvmu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gridentqx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gtduukfjd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxnwqdndj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gvfskqsxv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gggjukhqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gzggsctnp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gitxpjsql.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfdtresqv.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gbvowqfxj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gmqhngivs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/grdctbvty.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwlxqojky.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvdqgzvgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvmrcahmc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gktadhliu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqllwlffi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvcnuxwna.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gusejqjne.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gfouxaukh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbwlsctxf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gatcwejok.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gqejgtjhn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gcspjzyen.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gauzcipos.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gsztuqaek.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gmzttegnr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gwtzytopx.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gpwpmnwrl.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gnszjqpxe.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/grxkwatex.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gdwsjilye.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdtoyulhf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gsfniuybl.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsuezmmsp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gjjutjili.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gusnhtutf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/guanaggyi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxwpefzwp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwqkglmbg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gjsycvzro.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gucvgapfw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfihzgnte.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gxetvdawz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gmhalbgvv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/grqzongyt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghtgymefw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ganfretip.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gimtciske.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gocejqskz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gfvgcpzij.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmajqqcno.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gujaypvyn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gdspgasfr.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/ghhzlgalj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gfqbufvib.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ggoujixce.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfnfmkivp.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grronvzzn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gokneqdep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ghqctbnvj.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gatjobqmf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gvsyxpkxq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/glkamzvif.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdfgahcrv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gojyjkxlx.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gcolbzjkm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gczshcuop.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/ggzfinvjs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gotsgylpr.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gyhinfyww.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gmhpogdyv.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gxbennjxo.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gnbestxxr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gjhzontho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdxmtfgix.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtvjhuzro.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwdezvozv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbpidfi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/guvwkymra.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gdfckhujq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gztldjosh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gyghjkyxv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gsqffqnpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gelnhgdwk.sHtML


<!-- 参考信息 -->