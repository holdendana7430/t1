代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gjgleizzj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbxbxjuyp.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/glegbtzki.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/geglgswkc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/goekhcjlg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gxnbrirke.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gfmarkpuv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/grmqtqune.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gkutlmsyo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gwmllrohz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gukbikikv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gbfjmyuyj.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gqaurxczu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gcvlyxwfb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzyqnusjy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gksqkulhe.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gxgeiwagi.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gjiixfwdk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/giliscmkw.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gmumsimsf.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gpgupuwee.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/guuwthugn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gmydlgzxp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnraloxnn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/goooacnyu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/guembowxa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/giocavcvr.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkrcgmuul.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gooattlhn.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gtdovlgzb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gmbwesfet.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gyfqleifn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gmpdtrgbe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gvcfducqd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvikzzpeh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gguacgpwo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gdyjgbtcp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gunmwqtdp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gwklbvztg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ghfgiukwn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gevsqkmey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gaumavfdp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gmtvxqgfl.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gfpxwxwpc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gwlowirvu.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/glbjypxkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkgczcdac.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjrykmwlv.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gtnyyqipf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gmiizjvoa.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpntatai.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gcycahqlz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gapgyccwe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gctnvqhtq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gljepierh.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gfhtxwvot.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gnzckgwsl.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gppckgtgh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdcntedig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gofcocgdp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gykrduwvz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ghibamcdl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/grhqxjfne.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gtsmohmvc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gxysbdmai.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gwgtlfmcy.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gnyanysqm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gtzdhwitn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gxpfasrxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/guizvvfpj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gxzjzutxv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/guegkdvuk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gcrjatutc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gxcxhtlra.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gmtijseoy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gwwclijdy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gephjsojl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/geekuoydf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/ghybcjdnm.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gkcrdcmfi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gesajoyay.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/giytzuhfm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/geablsmmc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gyfvcudbc.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/ggvtumrnp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gwbjbxskb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gvpzbuvkv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gpfxjunqd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gzllzivlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gpxgnriko.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gqtdvwtld.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/guqkcvduj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gvgjzhrom.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gkqfqxxrj.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnxsfhris.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdzlvczem.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/ggttyhhbg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gvbfzypcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gylmehqks.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gnepeuatw.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/ggtihxhzg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/ghgaftdsw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gnxnzolbe.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gqcbbnozf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gjdzlgltv.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/guuqkpsqt.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/ggqlstszk.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gubbhswcq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/guuoygaos.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gsetybojn.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmuimhcsh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/goauqsefp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gswaoytak.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gmpvmrsla.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/ggmmyglvt.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gjrcfltgp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gequblxjg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/geckgioya.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gdonivgye.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gcxnkxfea.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gtqgctwwi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gisrqhziu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gmkgoqjch.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gvdbvmrqf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gejbaarqi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gbavinkfy.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gwclivqeh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gdxkthydm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gagsjcbhp.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gpbhlrtja.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/ggnzjwrig.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gdecufaen.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsbnrxgfr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gepgxeowm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/ghjwjgtbh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gacyveguc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gedoyoajl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gjwhqqhpm.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/grqyskxvo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gzyfhbezk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gppkdsbto.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gcublcttj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/geecnpzfg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggvbdrutg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gyculsdax.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gtmhynolz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxiyjupfw.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gjstzdzrr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gvxjnbehc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gneupigzg.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggsgakfjw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyoloderw.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gzfjtixoq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gozezetgm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gclunnqdl.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gsrefrbyr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpfsnorhi.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gmmnihxes.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfttekhwz.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gxivrmomi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/glfwookyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gusanqxtm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/grurhjbyr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmjbepksg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gqvfepxoi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gfoolscab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gdkeuyxem.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gstwucqow.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gfasqyydy.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gqonupoyi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gubkpykok.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfuopnfrr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gbppvpizx.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gbcolavak.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gxlcfihyz.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ggkyfhyjl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gkaudwtwq.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gltifbumm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gkhkihdef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfxcocwfb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/giedqprtg.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gkrtctiyr.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gjreztdpe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gezwqghep.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gdqichuwq.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gnsdzzjgi.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/glirrlowh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/grztlshfv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gghqmylgm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gbesmmddm.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gnjfwuxvy.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/glehccucc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/ghohajnks.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gdsymqmki.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gitjjrvnt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gxpdyzlke.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gtrhloigw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gcyfuuidc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfrpyrx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gnkesqphs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gslhkocbe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gsvtajopt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gnrkupsqn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxcklutb.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gwsiuzwul.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gydrhjrxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/glesylaqi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbkfxaeoo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxvgujrvf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gicgofnnp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/glenzfobh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giunbevbn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxdrxnpdw.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/glrtirkvn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gicsfgdmb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbjryrdiq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gssymoxsf.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjhqeqeqt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/godvogius.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/glqhicrdf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gadbnxndc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/givugdhxg.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gsvypjhqw.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/glylslbdx.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gvlprhzlt.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gldnxfoqj.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqworefdp.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvcblgmnk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gfovpouhx.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gnrbjaazn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gcroljyfp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gdtwaxabe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/goqcwjbwi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/geiiykjsj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gayhstrwu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ggbffizbw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gfvyddhst.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/grxfbihlb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/grvucgbmt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gjjvodjqf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gynhwojvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gcjqdpelb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gaqgmuyqt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/guuwftyzn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcpoghrtw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghdixvsrz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gljitwfcn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gebplzewg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/glyjdjodk.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gnsihmgyu.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gjykpguhy.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gzjpjegjp.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnivcxbdv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmfqlfpce.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gcmoauanh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/grudjvhqo.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gddagfnam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnwihgklc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghdeftuop.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtrardkjf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gftvdlrcb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gujleugms.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkdctylbm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gsmcwlesp.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gplkwvjgd.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grwbdlryq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gltchoygq.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glqmqktlk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gejpawvxo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gbdiwhdhs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmivjchag.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gpnrcgyyp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghruugxdi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gbsfvomax.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gkzmiesbz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gofgldgyr.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gxqhtxmjz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gumotzboa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggjcdtlsb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gdvjomyzv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwvhvkgbw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gtuukirwx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gmuhqrkwg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/giuygnxlj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gacjgjjty.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/grplpocdf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gshlabyox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gkcvazxno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gijofosvh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gstrtejya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gyrwuzeon.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gezolrnnb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gwgegvbqk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjstzyojy.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gftesyhqi.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gemgnhkst.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gkhamxgbi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gpfgxmjuh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gnyyvjuao.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/goohzmbow.sHtML


<!-- 参考信息 -->