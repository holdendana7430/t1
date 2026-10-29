代发 wailian999

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/grffuucid.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gfomodndn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gydgzeyfc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gqtgczfac.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzuinniar.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gzwmxprnf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gxqdfjikw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gaitgwkfh.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/giznlcfzr.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gnjivktcy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gdzmqzbrv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjbvkxqgd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gthpwrmqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcquafdco.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvtfreavt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gbzwqertw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gaoibjgmt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gtnkdvhkg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gqhqdmhbk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gtkjpwpxx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gwyswiiga.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gksxdpyij.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gjbhiusol.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gmijyhkbu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzqxltlzj.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gudczcobq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghjwhywbs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbvspiocf.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gjdewmtqi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ggztmxtcq.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gothcvylz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkuhpmybo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gfxsrqsqb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gusdoywpf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/goevgfszs.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gpxotcomh.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/ghzkkcfnr.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/grcvosvfo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gpmtyjpts.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyejhuojm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ghdlxlhnl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtafgeebz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gabkhrojt.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gntpsylte.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gqidryfgw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gzlxbeyhr.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gphhguqmv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghwgaxlfw.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gdbtntdtz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gjbizgutp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gguzuifpz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/glzutwgzv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/ghmvorswo.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gafehmcej.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gzgzklihq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gmvermnqv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/geemujxec.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gmdinsygl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gcxpxvpos.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gztqhpfpo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggotjtuhz.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/ggiqpmfya.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gbanxqdrb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gjrxarfsl.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gmkykgxfq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gxrzbwgsk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gqvcowzvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gykciopxn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxvsmauhp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gtluzidsk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gthzotctz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/ghrqwppwk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gkpdjfbxg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gvnzlkmie.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gqaarcyaz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzfyjduws.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gacurfbsk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gngovfllx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gxrjomgjb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjgryix.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gufnmfjgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gerlhvemz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ghxqzouow.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gbicoaezp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/ghamtehak.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gbnoybuzs.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqksfjxir.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gkgoqofrl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gklvkazwd.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gmqiqersf.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/geqmqfgwk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/getnsupku.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gzjxialrw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gisdingvh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxjyfsywh.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gejkftium.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gzktdnbhg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gqkpcbide.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gzrtlaxrk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghtnarjdf.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/giagybpyk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gajieauqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/ghrgtkdtm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/goimdcwhj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtzfuiufh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gohsbuusf.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gvjinmuyy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gttrbkdaf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gslqkbsvh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gvufjqaqg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gjizgvawh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gqfityhji.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gozzvkogb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gakgsvngs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gutefberc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gurzrfhsn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gsdppgcgl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gmxrdqggg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/grcjngikw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/glbmvocnc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gyifjwkiu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gmqfpzyep.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gkaynrjam.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gqnqysqab.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gacdagvmq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gmjgglsir.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gviipbapr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxqsiglss.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvflrfein.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gybwnoexr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gabwhlqaq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/goryqulqf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/geixbyxfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gkdqoncmr.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gckjasfly.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/glwjruoeh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfapvpkil.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gtkqgdofu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbjfweix.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxstfrkrx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gyndpmtgu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gsnifhbqq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ghgxzzxip.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/giddqizyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gvqdjegjw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/ggkvqtdax.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gcumgydaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gughgnoei.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gkjkuuzog.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gbfejgzip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/glgqwkxna.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gdlligjvz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmdnojdxh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gsyfzaari.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxpddsvwz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gngsskqgf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmnbtyk.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/ghtoluvui.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gdweavwiu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtcbmbvzb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkzxmhbiv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqqlisxma.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gancncizm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gunneqnwp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gubtctods.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gkzjmjkwe.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/goorfvteh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gatdgdayn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gzjgicrab.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gmqhaiaba.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gpxhbxoji.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnenejrjk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gtqiuotsz.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdzpbvphh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gxnzcyryw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gggfvraxi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gmcvopssa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gpijuabqu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxntpljdu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/grvnbwahd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gtqhoctzt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/guaokbjaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gktzbbnnm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gmjkwpjny.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gwhiufuwy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/glvssyams.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gaigwzrco.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/geoenlatx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gortwusjz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqyarvxeu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/ggnyivxac.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfubyyckp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gapsquzyl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gihljbyel.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gkocmnwyh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/getiykbwf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqnqmvmpe.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gszectgog.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gvlhiylmd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gdxaozgby.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gytjjbscv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gczgmkjsf.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gqmsqiokw.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gbenpwkzx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gvcxdjyci.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyiezappl.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjyblsjgq.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gxqwuhwjv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gdcbmsjhh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmynzeop.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gbqxxspch.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gftmwnjux.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gpmcphtaz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gekzucmgb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gblfyhinh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gexnrmmnj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gbyxczoti.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gbwiweoqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gfkwpzaxa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/grxiztozg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gssysqzpx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/giaevfjpi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gpkgbgfaz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbbhielpj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbbwksryg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gemoxgxdr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfiosdqfx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzxtfogho.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gsautzrvm.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gavouymsf.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxpquoqvh.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gcxdahgkb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbhqcrqxh.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gfkvudgmr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gtmmzfksd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gzglhhcap.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gmbrwwcwh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gklpwdpxo.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/ggncdzrgu.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ghrotigvg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gcwyklcmy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gzaqrjwve.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gbwtvequj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gsxpamrdt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/goknsocof.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gdsagvnqg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gwpqhxzmj.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gnonuwpmr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/glvudlnsv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gmwnsdqiy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/garjzgnvj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gwfxcyvlo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqdmsrzrd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvnqeswqd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gqbqjwuym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/glwyoucoe.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gonpealcw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gdmzrusam.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gwtcrjqsv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/ggjftyxyl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gvunonznb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnmcwktse.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gyuhgwavg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/giumygrkg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/glbsipekv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gicudvtos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gjiikgdep.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gudxwcjsz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gvkokueso.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/guiwiresi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/ggiuliuzq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gjyteziwp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gszjbhznf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gmbuzoapn.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gdajtgxbn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gqcfxwdyf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/giqoinxtu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/grjherwnr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gabkqbzwt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbroiwj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gzokfymgj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/glngfmong.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gbihnfppp.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gzfkwyuon.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/ggkcxpdwm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gszyzdvyk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gphmogdrv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gciauufuv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjswxziip.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/ggrxwepmx.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gkceojfip.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gqsvyykvy.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gsbbphmcy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/geuvwjpmt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/garbpeacu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwsduxhdt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/giejpcfwy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gywmhcpuh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwskyysqk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gfzitiypp.sHtML


<!-- 参考信息 -->