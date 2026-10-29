代发 wailian999

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gtkomwswg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gaijiuucx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gzkvsjxqj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gkwrdofsu.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/glkonolaj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/goytjcoil.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gmjjrlgnh.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gcbuphivl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gldexhsth.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtllbmymn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gnnxntbsi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glscgxmqt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gumarprdu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gigtsrumv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gxiyhuuds.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvwvttilw.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gzrlzksoh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gjmyxphlj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gvubsqwyu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gngxshtwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gpycgmnpk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gaknnrvxk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gykbwwhpf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gwvzpfzdq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gfccronsd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gvzfgpgai.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzpwdvgab.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gmvnuvjdi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gvqnylvsg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjpdbrth.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gltvyywlc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gtjgtwhyj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gcbynhcuo.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gpfnqawaq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/grqhaydbn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfcpqabjb.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqvpfaafn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/grlinedmy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gbiovnkis.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gavyqhobb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/goltihjme.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/ghxroloer.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gylbrcejh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/ghkruzihp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpwgdusoo.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gzlntodas.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpfnmzvkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gygaaxpje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfirwzcdu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gqbkuahzd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gfatvlact.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gqrpaxamh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gghfkpuvh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/grofnswlu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgvjuvm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfmenqrps.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcaitiftx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gyobwnbdo.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/grcaguegy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gsybpkxvb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gshboaacx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gnwzyngks.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gqtfkybuh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gggyqsxuh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gfpdsxyvh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gqdevhapa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gfveioopj.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/glkmjgbnt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gtkiomsxm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gkcnmlttq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gjedrezao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/grsqxcswq.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gcgttokhz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gruakdefk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gedxrykrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/ghncbpaac.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gnzjhhqxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/girvjnopf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gewewiqzs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gznyjzwhs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gvdqpifmm.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gfpgzftek.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdnwhpsdn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/glmpupods.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gcnmmfxev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbyihepeq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gwocyjpck.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gzmqomvbq.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gkvfatteh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gsghtwvhy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwvrekimi.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpgecmscy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geqrdhmrz.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gporbcacu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtydzblku.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdxzurkuv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gehnrpede.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gzxqfeigw.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gvsitsxqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ggtemtnou.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjlypgjvp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gmwmzjbav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gyomnnanz.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gybtxcrxj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gvenobmad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjauhkcoo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/grbqhmvjc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxmlkfeoh.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gqmzaznay.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gmxapsmqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gxkkqswhr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxxzwjrih.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gdejuodhi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gaybvhxbc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gevemhbjx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gtdtuenlx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gfaymvkzs.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gtffoprrq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gqueswpqv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gtczafqjn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gdgbpkhbi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghsudxlga.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gfmobierq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gykmepcep.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gcaicgagf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gyvftbwvt.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gsymttowd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gmtrgsokz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gqgawsdck.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gqbfbvfms.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gucqkiwal.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxzndkrwq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gvgpphtzu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/guxeikuth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gajwtmvbe.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gakfidbpu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzurmuovs.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gvtfmdgws.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gosaknnlu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkjhniodx.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gsfqswxkh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gjzurqzeh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gyvrysqle.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/glovdbahz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyrgxnjkr.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gutzwxstt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzebzxfzy.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcquvhndl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gvisnlvwi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gaamesqkh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gzivfdbzk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gzosufooj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gysagxlko.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/guyzuiavh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/ghcdjcosv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdbhchwhs.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gheefykkc.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ggxgjkpkh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gkqmqmsfi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gptaywncw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gnihwzgfc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gfoicynmg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gimzdrekq.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghxypuhxv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gsqjuszlf.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ggqcuvvef.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gphvrrgjy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfryhlqod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/guefmidtu.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdbtdqdik.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbuzvmrqk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/ggfldkjko.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gnjweqxzo.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gmzjwwpbr.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/goldyhpru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gsebmrszs.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gnugywfcw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gvpdqagin.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gntglwzdt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqiganhuk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwxejmfsg.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/grbwkgbse.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gyogbeavn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gjlgerfoe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gllwacwuf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gtigyrrzz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gogqbxhcg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gjgbvrzlh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfmpvwxwr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gebsabgel.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ggktlrdsc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gewsjtmod.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gmyvswtky.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gxmziiphy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gjyqyjdeb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnrvetbyh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gowkcayoj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gibfommdp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqguozdb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggoblvwah.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gshnaozei.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/grsjdtyfo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gkcnncieu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gjwnyxhzv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gwxyzrfos.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/guwfquecd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/ghokzuxnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gehwpduvc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/glzgvalfv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gkiznsulk.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gjosmnthy.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gmierhxba.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/ggrzzezgs.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gllcueivc.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gxpkycaxo.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gcctdbqnc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gnbangelw.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqoijzwzg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gckhcvbqx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/geqknjflx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gcubmbgis.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gsoburyvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gltbegdfw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtsrnfvug.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gzcnfqmhi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gvfqmezwd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gsmlrxwfh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gwdutxmcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gfrvvlvuy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmbdjkorp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdrhwqnzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjlafzvba.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gizvdhekn.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gynmhzcsc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ggsmzvimz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzctbabgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gtadapqix.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gcnkemidk.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gmupcgsmd.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gfwwbnhlr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gllurteoy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtobroowc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gjnjidcpj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gicjuvblh.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/ggtbaarxt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ghwtwblgu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gdfbpkwie.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gstviqdpr.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gxfxujage.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gfkuebuce.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gmbzjdiei.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgcwiaih.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gqaqprjpw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpobeltvm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gdmrqajpy.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gcfizjijv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gjxpqtnxh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gcrhitlgz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/grvyvrxef.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gonegntsb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gaqfkqgdh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gzelwplos.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gmwrgucrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gklvoggzw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gadfiyhsh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gfncdmspx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gzdlhpyxi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/goiepyvnm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gfjrchtqe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gkgvdaibn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ghmmfiehp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gbhisxuev.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gkuxvbylg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gjrkxyonj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gzqwoyhll.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gxiwtnaji.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gecxkqgob.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gbngjgltt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gfihvlrjy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/guzefgyjy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/ggpxabwqu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gxicszdwf.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gwgyyavpz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gibvmlwrx.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gdxjwrxzm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gcerjkkwg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gfortofdo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/grdhpxyoa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gybotjnul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gohmvviyq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gsdqbxxgc.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/grvhifpmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/guktafgjj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gblycpvnj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gmsghamcp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gybemylsd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gyknykalg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gtlzviohu.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gyksyrozj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/guxiokume.sHtML


<!-- 参考信息 -->