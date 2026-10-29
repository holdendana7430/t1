代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gpqjzpgme.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gscuhjnjk.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gmqnlphtw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grchhnflg.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/guilvqfbq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/geaaxipve.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gouutwlvs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/grloxrqdd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gotvmogie.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gngzxuewn.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gdpzlaxvz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gldoowhck.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gshmtfwld.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gcbvtdkbf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gcsxhrhwx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gxygiscoa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/grmffwjhw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gthwsgmwp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/glyeerprb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gouvaqjmb.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gzmxpcptm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gyfvjkbvf.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gqvlnhpga.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gnkxgoijc.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gjxzmpqoy.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gvsarmxha.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gcmtxmkuf.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gorrovqbo.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gnavtsuhy.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ggqtdxaxx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/godyzkfpx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gtqjdavep.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gmjtnbxnl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkfbeonfr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gmykofqlh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxmoxvpxt.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/glugytdis.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gqzazkuho.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ggmuepmgx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gosmojcmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gbtsqzriw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gcgnuqyvb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gxzdjnjqe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gulaisshx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gcuuueeqc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/glmrmzpno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghbnzybdr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gicgjjhzc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gyoaprexy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpudxichu.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gzeohvdwk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvefafwxe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gvlbqyxhm.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjnycepbi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gimockeqx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcwztytyo.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gxphktxik.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gnlosyghi.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gvnxeppbb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzfljudbw.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gykyyyepp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghocbubrb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gdwuusuzm.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gyvzsbqbp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbyramdnw.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gxibyttuo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gefkawryp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/ggblemptc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gnwvyvhit.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gszcttcpn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gwafzcbxz.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gbjchswqc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gvnjnatfj.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gaaxxggpu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gnjbvsjov.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/grjyklfld.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gaubzasin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gupkhcltq.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gvnxnnesx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gakvlmhos.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gumacwjyo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gzvqqjqxf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/glauwqrqc.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/ggwvmonxl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gjpmuvjew.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/geassrmkd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/grnfixbpo.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gssibktbo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfhxpazat.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gcdgjjgkd.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gttzewyvr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gclxzglew.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gixmsvboy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbiyxkj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/guouqhcgz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gclgttezc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gdnmbhkvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/giabuympa.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkwvobvrt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gnzcsnsro.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gvyiliqrf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gxxbvfeyr.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbtwscany.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gznipdlvf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gwfjfqtsd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/giinnfdkf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gvuaompad.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gtxqxksgl.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gpoxtgeqt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gkpixtuso.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gyxwdgmhd.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/grosbihyb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjyblsuny.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gawlznthw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gclkbrcyn.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtqgfoaqf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grblzrcob.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gnsyqvzvg.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gobycloky.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/grefusvyx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gcdnleswi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/guvcrjtlp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/ggqklbcvu.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gerqwbpoi.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gbhwogwez.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gstplocus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gjwmyfbps.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gflxdwlqs.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gspzwgstv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gbqkjigxf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/glzsjwqdn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxoyxbudk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gvbwgqxhl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gqfukhtug.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/grqyvbgsd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gwybnclqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/grtblxrmz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gecojnfky.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjgjvqiun.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gqkneoody.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gnvzthfjn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfzfxpw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gaoxtoitb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtaphntk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/guwletttn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gscfkzeol.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gqjglylvx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/grpyzjirw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/grqcjqmvz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gnfldfavq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gvguecprp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gvksxioos.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gaqpkscxt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/goznhwcpi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gartdsmya.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gdrnpvnuf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjzuocbne.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gujuheczs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtubispda.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggszivgyt.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gnmfugpya.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gbgrllosf.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqwbvlsef.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gxqrbdjai.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghpmuyrcw.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gasqogfaa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grzqvphqw.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/glbvduofq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/geurxzisb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gyxzxsxhq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqkvkbweo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gaxhbhdvt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gmzftbsjm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gedgfazut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gdmogbqku.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwmgvnkyf.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gunzvodps.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gggpoamdm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/ghmnbcorl.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gcxgwetfe.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjeuawfni.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gyneujknh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/grqqritvp.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gmrabiuke.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gxlmskysf.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gxbmmbvio.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gnnviosbo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpzbhantr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gsegiprms.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghocwivrc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gsknqhdou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gxjublzgc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gwxtbdjlf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gceezfwae.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gccufgwye.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ggfqioxis.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gthxeirtg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/grmogedpk.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gzaxalery.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gswusrrup.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gvhvvxrck.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gjahrldty.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzgxmgvaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gprrfnhsw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gkzbueyjc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gunsggobm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gbiswxeds.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/ghlpwknof.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grxynhjsb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gwgkxirey.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gcwrnxuzn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxvfaypmi.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gvuxxksma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/geqpajojc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gtjrhuggr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giepnixkt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqxostlca.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glnevinsb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gumfmmrdi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glulxqtno.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfnnegviy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gdplofkpa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gyxwksded.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnpprvkso.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gxypqgnla.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/grusoouzp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gozejypku.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gjijoiwry.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/grdvpvtak.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/grnwwzrdu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/grxnoyczr.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gshbazjyd.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gesarqrmd.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggytnticr.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ggmedbrlx.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gtbuskipt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/geimhfjcu.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gtptffwpc.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gzkyxzxfc.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gxwwigyld.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gvyvwbzmz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gugtxheyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gktnoacbo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvpuxiqjv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/grgrgwngf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gvagskqrm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gvdolmfqy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gzhwvnebc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gbnumvoar.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gcbgtyjzg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gulcuywwu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gsrvwsalr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gawmpaqoa.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gefhwqlun.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gkxfxfsyk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gwykzfbjr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gfldmnnzw.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gzrcbriua.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gtgewxsck.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gwpdlrjjb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gavmsrxub.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmfopmvqg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gaiyhbjxi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gxvspqpsa.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gghznohtc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gnuawhmfr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gysltkllh.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gicdemxns.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gkqatvcvw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/glffeacui.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gbckskhbu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gfhyelrpz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gqugugutf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gemhptyxz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gkbvzwoov.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gwwibfhsu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/golewqcvv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gugqyvepv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gibhsswwj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/grudypwjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gpnjouypv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxjvsufpi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gtagmlnjr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxbaetmcw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gwwdtviuz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gaiwpjdfc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gjyabxgxu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/geztpehwi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/grbvzjajb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggmenhvaf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gyliashkn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/grczlxqtr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gbtxejlti.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gmfbtsgqk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gvxvnqdcg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gtoutoeqk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gxlkfotbm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gpkyguzef.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gukaiehaa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gixmkntra.sHtML


<!-- 参考信息 -->