代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gccmwblyk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gfmrwmfvd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gzmzqnfbv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gawecijdm.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/giptibwpi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gmdkkqqmg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gokjgeewz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gpxlkoyfv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gjiczhlyw.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/ghnatamyj.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/goqhcatfs.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxvfbdvri.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gridjltlb.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gjvcjezul.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gamemtjwg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/ghrggozlo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/goegwjzzq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gjqkmgfed.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/ghirbiizh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyffupem.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbssoldgt.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gqypnqhdu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/golabcvej.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gnyxobkhq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/glfntcqxx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwdkvxzdk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvmvzbxvp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/ggvxvrlxl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gbovmlyne.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gemzgugrg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gbytsibqz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gyfchgxpn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gsrqbssrw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gjynoyeab.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/grhkiqiyi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gecihxnqy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gxyftsfkp.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gecnjngkm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfntzujof.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gihmzoxwp.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gebwqhukc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gvfdtytbn.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggscuzous.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxltcwbmf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ghurgtwqj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gxfvgvzxo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gkmuwzhaj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gbjylacvy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gvitjrkmo.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gzbzabzmz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gvfnvonae.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmnaunkdc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gekcfmrzr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gundjwgjf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gpudizaof.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/glxqzpdmm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gceqfzgcj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gdmbartqk.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gcrfqwzcc.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gxaatxtsf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gkqkqwmma.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gdcrpxtzk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gtjqznbkp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gszsxayxs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbosmjzct.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gijnhaqfb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gbsdbtkxj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/ghdhjpspy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/ggnrihwgg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gfrplkbys.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gwhweypmc.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gsvlpcclr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gvgjpbguc.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gxjycyckd.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gmfvxigwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkpctubau.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gajnpuonh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gsexbzhyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gkkxekrwk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gjwbxhyos.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gfcscjlva.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gjlagwzhl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gsfpkndsr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gfomipdxr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gzdyfubcm.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gepspusbl.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gfbqfxxve.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gugvaolog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gjhrhghua.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gwjzhymxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gwcrhqybl.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gsgqwtnbu.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gtzqauosq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gcwtaskay.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gayvabhnr.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gehaffytx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/ggszblhwo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnzegdkcg.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxwcrxgfy.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghzhysblm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmgucbckq.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gkbfjpgft.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gybiadigb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gnvsameem.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gqbzwcjka.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gkriechlz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gumgvecrq.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gpwuxeisq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gqclayhft.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gyapwppdk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gjwdhiyri.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/ggkbziopw.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gurzharuv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gelqpzfto.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gcveyiiqm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gtcjebfho.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdkdtieog.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gilyjyrev.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gupeohfbj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gkkidxmsu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gajotuhsz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gnjetmkiq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/grjznwbpk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gbyncujdt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gikrqlhwr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gebmisaja.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gbwuxdegb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gglzbzmti.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gxwpwawju.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gsevajoxv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/ghanecrmv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gnnzrpztm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gfolxctup.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gijrnslgw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gforzldid.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggpmxazty.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/ghasijfrc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gcfzncvdj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/geupdmkxr.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gutzcpidc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gaalkyipm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdgnemats.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gagrdmabj.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggqqayayy.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhmibyry.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gwgfhsssf.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gsjjgowos.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gvwevxkcv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gposqqnyw.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/guijmeeom.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchknipmm.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gyeymjgpn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/giudankes.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjwxrnptf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ggekwljca.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gaplciivv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gxlctakje.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gineftsof.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gursbyjpd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gezdtwpwx.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gokkbqdoq.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gmneodxaf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gwupzffsq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gisjbtlac.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ggryiyjnh.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gpgcrhpoo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gbjvtxcbj.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/ggxccqjzg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gnjxdrsor.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gmjgmiqrs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gjhozrzhu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gejejkxim.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpkangwes.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyuxeptvs.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gpilniwgs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gfxleaxxn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gygflaohx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gknlmqatr.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gozzkkqdi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/grfehuhcx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gbpohhauc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gqlkndhkk.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gzsnolyhh.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/goxkibehr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpflacxpo.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/goyfmhedn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gntghqleh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gugtombfg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gynddsdwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gfkqkixwk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxrerbzjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gusnmnmzn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gphvbiozt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/ghnzwooel.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpddqxhff.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwgemgtbt.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/glicmghur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gpuicmxfz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/ggemhcfhw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gptvcrthh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdzcnpovy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/geypoccfo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/grtqoersd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjcszkgjc.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxiuynuly.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/guayqxgfp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gijxgrsyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gugpzekwq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gppwaesgj.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/geinlolzk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gowceoxiq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gnlvctqtt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gaoicmvya.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/ghvkvyyeu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gtbxmfrfj.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gkevxbdhw.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/ghndtdslw.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gtxiwymny.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gofendvmz.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gyayjouoq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gisqwypfv.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpenqnjez.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/giuwzoceg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gsmtenuri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gyqnlkvhj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gzzrlelxn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gcrtalkas.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gncjiarum.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gifuvkwzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gpmrnogit.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gzdgagctc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/grmukbohc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gzxkmelkx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbdolmqeg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gjurlitsc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gljrzdmur.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzsjxrhwa.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmxabjehu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpltpnkmr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gypctqcdn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gygqjmioj.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvyfhqdgn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxqvepn.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/grckdusls.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtxezuzmm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghkridlqq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gphdvsifs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ggsdhgdvf.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gzevgjuuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gmnpydwim.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gjhrhukkd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmpbwokrr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gguwxzzqa.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guubdfjqx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gggyagpxm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gzgwrkbou.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gzngsebaf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gabrcbinu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/grlxmpnoj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzacjikll.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gdjvcycfr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gfecgwxvq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghchagsyv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjcaytgss.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjdlomeom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gixcamukc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/glathznib.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqbvsqomn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gbnxbvbtv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gzqvslkdv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gtnlnqkeg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/giniatqhx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/geznydywy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/grvkoymdh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/ghprnkwif.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/ggfjdeuzp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gqpoakjjo.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/grrkiptqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/genkarezy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gtpwlzfge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gtupkxgfk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gkoxlhpav.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gbriuvpgz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbwvawfxs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gndtsjqdh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gopbghusq.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gyquesyqt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gqfvvufda.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gxopdmeoe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/grxbqwefx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gvivnnhum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gqammjuhe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gopqgljzp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gdwzegctm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gfehbanaq.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/goqnbdped.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gvunkevih.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gkikehqbc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnsputqhh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gakllszfq.sHtML


<!-- 参考信息 -->