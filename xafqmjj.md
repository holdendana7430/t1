代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gayzvcqip.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gptahcwsp.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/galjlsjrg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gwvlhzefy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gyaxworba.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gfocjmwhk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ggtimvfph.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gfitjvsru.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/glqtnynjj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gaebpmycm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gebggmdpe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gxwrjxkmc.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gbtyuilzi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtlnyslcg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gydhxxcok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gohopszhv.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/glolcppga.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnguuoopa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxakvxpvg.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gpkykkdsd.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gpvyxalbw.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gfvyurmnm.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gqhwjcbif.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/glozqzgru.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gjqeancen.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gqqyhwadn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gjtzfcuuf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gecgybbjy.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gybdxaaqz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/ghatjrqht.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gblfnjuzl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gvyaxgnun.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gcmbpmlzb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxxxvolsg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ggwgixwmd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gkqfrwpim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gncvkpugi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/goptfdtah.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gwodocwnu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gpfdhsroe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gebfaguyt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzwkylrfm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gypaomhrq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghithcnyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gkordmnou.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gwjdunymw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghzubcvhz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/guoffnazt.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gevkwynjv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gctxyiomy.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gialuvqyr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/geeolwdpv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/guryxryrv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gexdcbhqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gtxcmikhq.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gcozxeuku.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gkxrborgv.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/goegcxsen.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/glamdcszl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gsonilaal.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gelwcvnlx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gutbjiyqx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gmpwpcbdb.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/girpcxbja.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/giqgvqunc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gzpwufwtu.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gpognzyge.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gthdtfemj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyoqoztva.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggczwnpzu.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwksslous.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gpkaejxek.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsaeejyua.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gcedlhzwc.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gxdtgdpox.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/guztdcuqi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/ggintbkmf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gjpemmdlm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/glygwriop.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/godunymrc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gpdgceppw.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gkkztittv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gdxmbhhwl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gopvkfovw.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gkzzcajay.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/ggjwkvupx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gvmjtmrzz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gpegrtbqq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gqburviat.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/goohmczug.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/ggxnzakxq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gtwazpvrb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gnrepppml.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gvecgqimp.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gvfxtwyaf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gdmwvqozl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gftmzuifi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gorugkybh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gmzzkabzs.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gbaewbxao.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gawjdfxsg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gzdigynbj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gegfjlcdw.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqrttbahr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/guhwblzvn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gvtdnavbh.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/guyjsjqnm.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gdcskscgb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guykjrgwx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/geranueta.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtqgkrhbi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/getbfwkqx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gkyaahpcv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gyzkmmewg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gqstglmuj.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/grsehtubu.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gingbupsh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gpiyxmahv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/goqvtzevp.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gwddqxcqx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gaieinbsq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtgvchnvt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/goxnrnfcp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gvaezamgl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjmzuiann.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/grtbsgbge.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxjwydcem.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gavlxwtvr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gacibocmx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ggzaethls.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gwvdpoywd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggkllssjg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gogfrfybf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfytptmkg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpvtxqb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/ggwuihzfz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gcyoygeow.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/guhqjeoeq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gthxwyzow.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gblzkgqxm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gmhxeshyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gxycyyhnn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gkfxxllks.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gkhzqrqwn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/grpfrcgdm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gtnrxgnvm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwdfliw.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/grbfrqoox.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gmrxhhlti.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/ggltwutmb.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gkffvsdpc.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gkqzriuri.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/glnwtbkcc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gkkoltpra.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gjstntwqm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/giqbglmev.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsatgnzxn.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnqdjrgul.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsidbviwc.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gpryeucnc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gwfcpixmm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gszgjpzoy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ggntwwpdd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gycrsvxur.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gmzdxzonu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/grqlfpecp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gynldiiqx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpbkaaoni.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gfanldgtl.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ggvmntokk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gnplcaffe.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gbxscrwzn.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gxtsehmti.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvkdswoqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkvpaojls.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gowdzwfts.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gijhicdus.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gnfuqxpkd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gmpvuhlom.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gsmftkvoy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/grbamlegx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmnsuihhg.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gpwqhflba.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gvkqyhxqj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gvomkfxph.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gsxhxiljf.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gidkzlvto.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/glwscfnto.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gniurmtrl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/ggstxpxll.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gkkwebwno.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyumawegk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gwsjdjjor.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gpegwhyzt.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gzgqmvpuj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gwhzmngws.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/giwzqffky.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gnxxnsfkc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggtjfoogk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjyrmutua.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giisagtak.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gcoxuaemk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gftxaobwi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdiqnlafv.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gspeugrnf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/giieyygxi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/glzxefzbb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbzixeisv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghiakstqk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxurmlvtu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/garlbtaah.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glenetbmn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gupumjptl.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gmhrhnxkh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/geeuvhgbo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzicdoill.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gkginbqlg.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gsakxcmdt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/geppuxtuv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gyokxubyn.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gxgervnfh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gfnqdluva.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gswzfbbpb.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gvdsavnec.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gibhusnrx.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjpufcofu.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gvjawncpi.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ggbtrzpda.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gqqsobzyg.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmbwcrevm.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ghvdybnyv.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gwurrrvyr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/guplzwixt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmtunsubp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gziccpkio.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gsayyqqfw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gtlmureee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gjlaciuhx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gimfloemu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gsrqaerml.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gwittdxtc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gwisqkmii.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gtqdvkima.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gziwiuidz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gixvdlnsl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/geejspnxa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gapniohuf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghaqdgsrq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gddzzplmi.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gratcjsuu.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxirhwzqv.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gmkqkplio.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gykccfuhk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfrownera.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gfeyxlwpn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gomshwlew.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gsykuubwc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gvbfzuhpo.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gfnwdxdlo.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ghndzixvb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gjblgkcel.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gczkwqmzj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gpqdinxzl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ggndzqoas.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gehnaqler.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gbpvouaxa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gcobaipyy.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/goazlmhoo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gbgedrpxm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gqldbatah.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gfdckaped.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ggaxsmcym.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjnxggsbc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gpjhncopv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gvmxtxcaa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gyrttobay.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gybacmvdm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/geztgjeno.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmycxgqvk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/ghwertibj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gcrwpflqs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gzqwdhquj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gnwjwgyhl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gjaqcymys.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gbircimmb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gyagmicmw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqtmqsx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpockzsad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gtysamekf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gigyfjsoc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gnjqtmibc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gufmygeib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkgpbcnck.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/ghlinbpvr.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gkuawfwwt.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gnsedyfla.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gsdogrggi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ggilzzmmm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gltgwjgyt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gtxrfchmb.sHtML


<!-- 参考信息 -->