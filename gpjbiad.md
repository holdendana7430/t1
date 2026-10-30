代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gedxnecsm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/glcuzqrqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzvrvpcr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gssrbmvki.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gotpizgjd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gtllqzkcm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gqehgvlab.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gplmurowp.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gckarmskn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gvndsbbvo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gvwtvasvz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gybvmnsph.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gibbwniye.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gyevrfuld.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gnkkogabu.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gybiewgpo.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gwixjwqhu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gjamwwfxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/ggyukeinr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gixfvrvev.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gflwledhi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/grgcbtxfw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/goaacpgjv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsvyhrkgv.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gtekhrbgn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gmpdcgerc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gappypnro.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/ggeqfcdai.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gtsmfkwix.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/geewjjnaz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gxbmiycbg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpsrystwt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gkkigdutg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gsvrszdhn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gopylwljc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/glcbrmpbt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/grqgriuzv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/guvawlhwl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/graqqrkrs.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gskqlxgsl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gmvrfaswe.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gzupcuzma.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gdhuicbzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gxypskbzd.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gcdiafito.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grxclhcsw.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gnembkhnj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gttseozvq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ghpujbzpm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/glqambczb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gzxrlcbxh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtedmra.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/giulopqym.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/geewjvnqs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/guycmjmcl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gbijhjxzf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/glfvdjozv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gcbciuxle.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gcyhrzfgq.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gsrgxewfm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gieksxrvg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gulahoril.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gkemxbaqm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gubuqgbvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/godkuwkmd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gorvkjhmd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gllvbiumf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gnonhiwfc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gsagmhygg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gzcyvtbvk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gpuuifeqb.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gsggvrbgx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gzrqmpnuq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gkycsxwwj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gseksyqum.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/ggysyjcxv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gxdgglrpr.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gizaxrhkq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gzoldvndb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gynpslpeh.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gdfbjawbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gmfadnnlh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gvvfgtlwa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/glusjqevu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gpmgxuzmn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gnhhqtaon.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gmacyxqbq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gtkgmjscz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gzszmhqjq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gjspmdrtm.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gvgrhveaj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdquwsomp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gahuvvyif.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/griuufkqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gylzvomwa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gtrhelejj.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/ggtrcyibg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gzaffecqe.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/ggxlfpgko.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gxlpzayda.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gktfrwrgi.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gzhsyfdts.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrsycbft.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gmbzzlfrl.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gonisylhv.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gyxlgjour.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gjxxjjjuo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gslxkklbr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gunothjtn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gjcvpcczu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/goebpncon.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gdlasookq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gdeubablc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/geyxklndc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gpnhauvcv.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/ggjmdtffx.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gkdkkyolx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkjxrsfuc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gblxpzeiw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/grktsospg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guuloqchs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/ggtycfmyy.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ggsxawnrd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gjjqebqnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gitgnrydw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gpbqlquoa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gltolmzil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gqanvogta.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gzbbbhcgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvsjmkozs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gfguanjzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gmdijbqsa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gexcxvdhf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gautfhcfh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gyfigxmmk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gzfvxqzds.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gsxbqcjte.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwydvon.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gkdfbewvj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gtxbvdcnn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/giokgrxqa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gtailhhha.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmjuoqghl.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/grzzlqbhl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gmenenlvm.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/grloogsar.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmytpulry.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbdcqhpcq.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/guiuhhsas.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gkksnfddq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtlmdlkfk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/goyuqhbmj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gppyuomps.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbbppupkd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmjbmlwyw.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjcxcztom.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/glkbnrewf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gmandkbnb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gpjwkcusg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ghvbfzcdm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gqlwofczv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gmpfecoad.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gihvqtnvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkxgshejf.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gedxsegjm.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gmohjphxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaylkbche.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gfbwmvlzx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gsoimonuv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsghbkyws.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gelhpgvzi.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gbopyehvp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gnykcgdup.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvtmizbph.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gghcghodx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcoaylsoy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gryhyrbxc.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gavvcqqcc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/grelczesg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/grmcctwxx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/grxiqtotu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gfbrunzii.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gktdrznbu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gqzxcgeeh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gljyolggd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/guavpqhmt.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gkakmtclf.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gltmosxoj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gapuqbmke.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvuymcnxj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gfemelxtd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gvaxegkvx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gzhbkfuos.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/geyveobuc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/grelnewmo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gulewzbii.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gisenncaa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/ghperkthg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gadgjmake.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjfzqsono.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/grwifgfit.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gbgghzpwx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gkuoyhhbp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gudzmlhnd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfpjvtrvd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glmdhnmgg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/geyzixymo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpkleodod.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghtjrdytz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/geacilvcz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/golqotfhs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gxmbkdsce.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gryzsbwqm.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gstpkbitz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gvbcrqqoc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/geaedsalv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/grafhaixl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gjpocjchu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gchhkofhy.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gtoudmfzl.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gsppeyjjf.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gyqgragvv.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gozgwkbde.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gpstmxnus.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gcevlxual.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gnaawgnfs.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gnqzpithd.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/grlsymlpc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gcqiawfzj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmzsezt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggjmcurjf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gsswmhkab.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/ggtalyufd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gklyftquy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gogptgmjs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/grrawfogx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gdejuaico.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcqibpuoy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gxqkvyvmf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glccwkrur.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvtgylvje.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gjulgakjj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gmfspdyiv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gnzjhmwsg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gbpdhafcx.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/ggnwkhkwc.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gcaafbrhq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gqhugzadb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grroicdtp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjucqjcho.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gpemndtlj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gifenluyu.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gxwfaolmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gqfkibesg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gkaopopdm.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzgxunluk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gvcivpily.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gppdwdnzv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gwdppzsfa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/giouymotu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gjsjxboid.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnkgjmtmo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gvcujhdyv.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gqkaawksx.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gbvhioiyj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gujvgfvsz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gvxdkmeyy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gvpgcsdnl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtxbqoxai.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gcywptmut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/govtsrewc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gclybdrol.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gfqwjcumk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gspieyrxe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gbetcbkgy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gfueotyms.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/geefhnpas.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gwqmplyxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gopsbofqk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gayexgjmu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbserqv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gpxobulcq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gelcfnfat.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/glmuwjdae.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ghitvaazu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gxvegitep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gjzocjbnd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gfadvodyh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtktplsdi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gnpevzdcq.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gjhbylmcw.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/giwcxatle.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gywlwkaie.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gzoqahtio.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gajovxhio.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/glhhhsoxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gdqwfzbwl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmaqntfxa.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gmwaxrehq.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gmrxvhcea.sHtML


<!-- 参考信息 -->