代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gwualstan.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gcjezproa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbgkpvtfx.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/galscqyeh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gevmnmwsd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gqcbcngwk.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gujstzhbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gfusravnf.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gargjmxqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/ggouzluyq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/govkavwbv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gnwziuwoa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpfrxhnju.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/glnywvqfn.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/glihmuytq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gyedirmjx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/geyjykyuz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/giuqddeba.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gawslkxzr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/ghjpzrjkb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gmmdrwkcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gzrrskzew.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gelrstodj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gwjjjidyi.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/goghawhpa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gtpeqamfk.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gveamndcw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gairatxnw.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/ghnambbla.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gadwzuwck.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gckxjkvrl.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gnbbiuboq.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gipzifwjn.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/grxclfaql.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gwrrojgxh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/ggflzxlif.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gsbyyhicu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gapnwkudh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gohnmxhcx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gukfawxts.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gigcwcsdj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnckfkgt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gccaotpgw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gmzslrvbd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gspbxbyno.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gaefecvwl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/glhgefrtg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gaaanbkul.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gcemwmwkq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gazgynvra.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grsbqvccf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gvcqtmxgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbwoehetn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/getteptnw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gkdqqsrgo.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/giertfiqd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gsdquaixc.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ggzfmpyju.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gavqekhvh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gacxonbwe.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gssbodphu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gmecdnvsx.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gybhgqhjz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gbtvhwbnh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdymgbhhq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gcasguuwv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gdbvbdiek.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gavxkxvpq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guwykzxoj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gnafxkbdc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnbupejmf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/godwuibld.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gezhbcejn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/guyisvani.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gbunlbtma.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/ggiyxmcem.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gyigojjhp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gysqqrvlf.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/glkoqzfal.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/guazlacyu.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gmzyowixt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gcpyvwpaq.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/grenzuaxw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ginudrcqw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/goelekgby.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gafckelkh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gjizbrylx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gvfzunqhb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gsrhdwmpv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gzexglxyz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gzfsxkyvt.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gojoworjc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gparbtxrv.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gzwzkodoy.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gkfiapnsq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gwvdtrqlu.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gwjmvrbzh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gqqxbpclp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gbtaghrxr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gwxywdxye.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gaudigvds.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gykkcmxuo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gwtrzviyt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gwufwmoqy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gahutiuvz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gvqqerggd.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/goivsqzbl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gboezcbre.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gwyocwsgi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gaqiviopl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuhxibb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/grhjlxkpn.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gwhnssgsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gsssnlcbz.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gplwqiwxk.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gutmaozvk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/grmlsvumf.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdzsttesi.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gyjrkfhcw.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gyzrajjxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjabbvghz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/giygprlzf.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/grxfymcxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gliaxqvwp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzjlwyzkv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gzsyhocwx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gxfdzmsfl.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gimcizhij.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gjdpqdwiz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gunwrybqx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gkzvdwnaj.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gfelolrba.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gslotjywe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gafumcmcl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gtyzubkdn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gwputtjkq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/goqygxnjw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gbrboojgm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gakthxllb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gnvfliauf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gwnmtywbw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gjqkttghd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gbljeidvn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gcbmpeagx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/grcodbang.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gedqruywp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/ggdwndmxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/guimrjldv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gfbqrkgtn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gqqskxhgn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gulcrwasd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gytegmtkj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gkdosihev.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gabfndhhr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwirhiwog.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gojngylgf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmbtiir.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gejiftfte.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gssbwpgjq.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gtewxbzzw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gzesfuztw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gitdjvylt.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gosvkdirp.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gvthctwko.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpihzyhbq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gwlybpgkb.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gnmvuebkf.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/glytbocnb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjrccocyk.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gwsoqmrna.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpoufmztd.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/ggwfgrlsl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gpjqvhzok.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gicukhlfb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghddejktv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gadevwjpn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gjornikrm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcbahxtzp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/guntkkypr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzfqgrvyg.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ggtrjjuct.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gkadvlaqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gwfcrbftb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmxtpnbel.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/glyfqaawg.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtnlokdms.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gluyboeff.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/goutrlzzr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gnazlfsga.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gweztvnwp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gteecnnnn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ganmujnim.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gktyxdwis.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gnosykylb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/guoydlvho.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gkcdcbqkt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gnnrycdkx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gabohhttm.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gavgknbkr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gpfxjmqwm.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gmyfhftga.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gnauetysw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gyfrhkkgh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ghmwgnjtp.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gnqvkkjwq.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gvflhnepm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gnnanhlcz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gcovakgqm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glgvrrrwi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gkagshjjx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gzboxcshc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gamhiaptu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gpdjfcncw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/geqbposkv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/guqnzfpyt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzuzprcpj.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/ghjjoqjls.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gbyvdkdim.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/genhoyghk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsacvqemf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grnskopse.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbcrxpdqo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gxbrvheas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqwiktpfe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzjhrohbc.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gkgpniqwb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gagaqbhzx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gadxirkvj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gnitcdxou.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gygmamcmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gvvrtrsku.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gukapsxqx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gssvtrzrr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gsmxjtudy.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gydfprgnx.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/ghixkmijp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/guzslkavk.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gbvrpbhnb.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gyhtgtaun.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gxhbgewaj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gjlkrpjva.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gotigwmcz.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvzewncgo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/geogsoidk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gfbrpbcmg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxndzjgee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gukkxliiq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gfcvhkvrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/ggtmkienl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gouaglars.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gaelscyra.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/guptnhaam.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gxgkkojxk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gjhtkufys.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gsucentap.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gpxdwycyp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gumxawnit.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbhivjbpy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gshnrhgwr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gpqoqfueo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gepcdfaio.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gcvrsirqc.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gxcvipghq.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gxauggesw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ggllyyjdh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjgecnmrf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gdqbyxuzs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbruulcvg.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gbpxfcxvp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gzkbjlfhy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghyynlmwe.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gpxcgqzbi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gwttidnqb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grhctgmnb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gymrkatgf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjiqugqs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gnkjsnomw.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gidpqxuws.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gsaxgnhqg.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ggissgxgh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gualsbkfm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gallumuca.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gelvesdnb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gyrntzhoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gfifjxblw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gvbmmscws.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gcfqmeafc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/getgdjrjo.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gukxamjgj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gtycoqlxl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gtxfzliah.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gyojdsaxh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gejmxzcaz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gefqkjabv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gysyvkgqy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gnvqqopxb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gqfblqhac.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gfcnghzol.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gypoaokre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gumylhirm.sHtML


<!-- 参考信息 -->