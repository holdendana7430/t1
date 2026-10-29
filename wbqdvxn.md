代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/guuiiselm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gsvhuuxya.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghpyvmpoo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/geitwiosw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/ghglniwen.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gqzhhkyil.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gsoysjbjk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/grkkatqpv.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gzcpjzpax.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gbudngmrl.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gionjprlk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gxkoxzbhd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gdpqakleo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/giajvwroj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gfgdpwnym.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gyjrbzufw.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/ggphcdfxj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gjjesffli.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqtemxlcz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gptgcorjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghjjdjygo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/ghzamkgcx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gqmqwsavz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmodrhvvz.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gzdpwaddg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gxhaavxqh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gwiracncd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gghithhym.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gxqqqxpya.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggmwydjtv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gfytarccz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gnynodtmr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gsgoblzvx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gtflvwqsh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjknjworr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gamvedybq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/grtwqaxrp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/ghnhhirbk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnrvxxriz.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gghqhkupp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxpqfsww.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gldbmtlxh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gokbgvpbt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/giyaajsvh.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gxtkyadya.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gamijkpcz.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gfneuzqig.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gukllgkhq.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmpfgomwz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gqnbmdhig.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gqyqiaesq.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gfqbqxoai.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtnitcpum.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gupfgfpzh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjrnvvocc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gyuxfhtar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqlkuwtkl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gctkgskpi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gsfzbxztj.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gsodttdps.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gfieiaopz.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gbctawkls.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gcsvcyahq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grxquqekp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gjhljgncu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gbhxwoswg.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gpihoikkt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/ghzqldexb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzraaxwgv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gfgckkdwe.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/garrdxgpn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/godsmroqb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gtmuaoano.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gumnnxrnc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwcjdbvf.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gzsjjdrrl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gpsghnrtn.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gaticggzm.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gorpjrueg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grzwapzkc.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gykhvcmhk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/ghjzbkdeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/giqxkynic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gnzgphqft.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxofutadq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gutkvjhia.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gymbrgydp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gdnzdvapd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/growpizbu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gcqelwprw.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gdazjvnze.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/galtjtdss.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gqdbmadgq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gazpbpoei.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gryreudgc.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/govwwgidi.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gskceocbr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/ggcqdwvdx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gfmzkghuj.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gcszbency.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gdwwfldoa.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxvnxphqu.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkybkwvpu.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvjjaadus.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gogfnsnoj.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gwnrsoova.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gdnavrwmy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gmxsvvark.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gjjcysbuu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfuvwma.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gefiajyas.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/grdoavfht.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gineabkel.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gcnrilbqu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gdhnhgrps.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gaxjbrahk.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/ggwcrgpfe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxepqpeqe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gxhmkyhtb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/glyyvhyuy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gaukpqrut.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gahnpqpjr.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwltntqmn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gxarcfvlf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/ghmpwpxvw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gksgguzqj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gyhffivnx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbupfydsn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gsfwoopfu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gulouvpuh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gpuxpypoe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gpwfaqpdy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gfqxrodfd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gmsgjfevl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gsiilckoy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/ghwdjxzun.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gbpdtdswt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/ghcohnvzp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gerhesnay.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gvvcxhbzm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gczogpsmc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gemvnqkbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gawkyjild.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmmczhspf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/guddrhvmb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gvdlcddvq.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/grqimagxe.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwpczhvzu.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gbvdtmclb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/guoitaxhv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gqbwrzjcr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gkcohfeqi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcqwsatwz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gebfcpngq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gowhgheab.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggiyqcrwo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gjmfbnoix.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/guqisnhbl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gcllcjajq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghnzihfrn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/ghqxodlux.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/ghnnuxpeg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gzlfghzjg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkihfifno.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gdeenwtbl.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gtigflwqi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gbnbawgte.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/guodxblxg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gthaizthe.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpfzoopim.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gwcaehfeo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/goujtvxfe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gvdjwgjaa.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gieftbqsh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gznypmxpe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmmtcoenk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/grvhmuwcl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gwruksvua.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcwabcnyl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/grenxotah.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gkfoztxzd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbuyxniyt.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gswszgzpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gvtbjssuh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gtksabanq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gkulercot.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gihpzksed.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gywnvnqha.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gqlwpoktc.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gpmibxuul.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyudqoszs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/ggqmmulys.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gkujcbsmh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gscaxiitf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvwllszxp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gyimmccfz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzdijfqyy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gashcprcx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gvpocgzrr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/geexvadqn.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gengbrqrz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gpinnbowi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/glhvggodl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gapzovvhu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gpbjtgvmd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzgrvowaw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gbotukqbm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnuhehyda.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvcayeinj.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gfywlfxwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gyinmpfbt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gonhodwmg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gmyyfuvid.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gayppncsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gwmpuoujl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gfuklzkup.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gjjeiseev.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gbglkoijy.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gxqtaswum.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gnfpizwka.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gjqxoayev.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmvjzkdsd.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grrncvkxn.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gmgtqbumt.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gahfmrtgw.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gntvekckl.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gscmopgxl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdlkrgz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gpdaimtcm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpblivmy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gksozozjo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gjjjbnkty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/ggkqccxko.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/ginqcalyn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/goeksssxl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/ghxafhmyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gdoxvhxux.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gkejxmrvc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/glfaolblc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvenafnul.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/ghgebpyrd.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gbwzjiycr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gazyfkfzt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkvxszxwu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gdzebuaiu.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyeebrdwl.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gjaaidgmh.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gfpwdfppo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gyvfzflfg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gimvczvdv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gdvvoenvi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gffusuxjm.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gyalllfli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gsancssda.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gxvejnkdd.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gtlaublcz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/ggcrgsttr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gcikhuafx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gmhweaccf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/ghnjpsaqj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/guqfqcdoe.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gzdbsakjf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gozadogaz.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guklsdcsl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gqreusdmo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gcejrdkpf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjsqnrszp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gotoeazqb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwundbqfi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/grjglsruz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gbhibjexv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gthteibxt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/ggmwuevgw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gqxebfdrm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gyafybysc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/graqnnhpv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqhvvpjxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gvqlkieju.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/ghlbymtwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gsjshfflm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gvlaksfhk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gzjppqdex.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/ghwckudaq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/guwxrhwzs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gebzkcscw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gtxcsurnd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gzqxkopmd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/ghzshkqui.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gwqcrcyit.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gkhbdxuui.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gminwprgi.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gtjjqlxyl.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gnzgripsq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gjkzayjoc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gfsyxfyuk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gdjwzyxuy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gzihnkeni.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gwikuvpph.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gkkrzqmev.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gzxvttiyq.sHtML


<!-- 参考信息 -->