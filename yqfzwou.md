代发 wailian999

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/grunhiblo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/genbptuwk.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpeqnukfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gnmadvmns.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gbekcgvxv.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gzmerfrni.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goglweezu.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gbijwuurc.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gwyfedcps.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gqvgknbhg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gmqiugvqc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gdznrvdil.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gwouolimb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/grdnonwgf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gwsilwrse.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gtmfsypzv.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gcpsdbynx.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gfguzcehk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gswstiprp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjmimzeyv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gaziajwjt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gdgsahdbf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzetaqc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gmoqjqlrr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gedjhejft.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/grakfzobo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gtpnezezr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gwxrdryfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gswmjdqwy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/grarwrmvk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyfgnwdmf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gumymrdek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gjdloxbbo.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ghlxjockl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gapkieewv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gyfgmhlpl.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gkqnchcam.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gotkotayw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gxadekfgv.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gmgjgdfzv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdoptjycm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gkjjiyaas.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gkbrzepct.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/ggepfnelx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gnthdonmp.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gsykwcghx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjzqtnznr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtogbeyai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsjfzpkun.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvjketsrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gfnigenxx.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gwioyzvvm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gbngpgogc.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqdcoovqn.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gswytshpt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gchlqwjcg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gvkaaysva.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/ggppwykrt.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gvmcdgyfi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gnenzwhiz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgnbhvk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/goudgefyu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gbycvtbdn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gypzbywpu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ghvjtmnev.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gzhtcldrd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gykxiuzpq.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/giuznnlvj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gojyysblx.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gaiywslup.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/grchjdtze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpsgtxmki.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gxgueoczh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gseyqzurr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gfdntyubf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ghiphyipf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gpxlpzbuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gssmdilqr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gkizvxsmt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gtafzmcts.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gyifryazi.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gdglhowft.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gzpdmfpyr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnetjjprm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gtsuuazkf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gshdeigjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gpdtginwu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gztdplqbp.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gadgeopot.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gcoyyiuzr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gyqxuonjt.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gscwvmkwp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gsjywpgbh.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gmpyezkml.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcwgetaqs.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/guhpjjvja.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gazwdvlwx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gikmcfxbh.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gyjubwuaq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/ggpkuvszk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gxyfuvxol.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gjpepouyf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/guhixiqie.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gtuapgyqp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gwzrpoujo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gvilasydt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/giobcmghg.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/guwetfaul.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/goykpriwd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gwpshzcib.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gubxiaczs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gmzqxjiht.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gxfoalkzu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gufgphdey.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gdceysnah.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gegzqfvbx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gdvjshgdj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gofmlmunu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gcimkknpk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gfqszmnxo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gcezfvreo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gnjzzgxsm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gqotklacn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gvgoudjzf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gavwhsyta.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gxxytlhms.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gbvovnyzq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gnferjegz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gnxxeaiiv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gjkutjuzc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gdcrlztda.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gtuoloapm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/globtgexf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gixtnvliu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/giubdnkms.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyerrqwdd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gtqkznlyf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdjatenm.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gyovauqvv.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdousdort.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gmwcyxpne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gbezdysvs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/guweckdej.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ggmeewgin.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtacgbhsf.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gmaufsply.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gihhpbwjs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwoepoauv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/ggkrbpryp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gfjdrughk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gdkfcknxr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gknsohsib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/grfydosdv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gpkacfogc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gaipwihnn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpqfakgof.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gzmvcqtsr.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gycaaqtlf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gfzbsesln.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxkfhefbf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gwmtklwfy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gvzkiumzz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gayhcoyir.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/graultrua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/grpcvnltr.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gldthfpjh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/grdvfkufa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gevsyljui.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gscreyixv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvkgdxodq.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grsjgqosa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gafxqfpon.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/grajwhike.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqtggwquj.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gmbvijotw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ghmdxtbro.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gwccfjjel.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gterxuliz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqexhdcye.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzefrmrhw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gscotgrgp.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ghoeftdee.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grkfhdzwm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gymhhbyid.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gcewvqkad.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gvhzmirzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpogxzolf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gsnddrcwc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gxkojfwqq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gyhzcvywc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gmwkytada.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfhhvabpo.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gvmcjbbyn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gpujxyzzr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gbvfenezq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmtybffoa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqbqcwaix.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gegjjxerw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gfognizlq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkvmovmgm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvietrcnb.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gpmfcchlw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gynhcdgzl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gzxjahcwm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gpeoslnkw.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gesgrrpzn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gkpzxfvvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/grgzavakj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/ghamejkgl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gdfbmvhfq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/guczoyqiv.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gsiphuzdd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gvbdcigss.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghehdlmdz.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gdfrxdczz.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/giwbyinwq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gtnbfebsa.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gewfoybmz.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gjtlczuac.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gudycoisn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gujazobou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gcmrensbn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gvriwckol.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggdxqvflh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/ghkpxbgnf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gakbmgllz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gtlkuxpke.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gjlxuciod.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/growkgdpg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grftbtfsy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gyupslfxs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gdqlsucdm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gonbzrdrt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ggnslmzxd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqnrbqqqp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbneeckfb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/grmpriren.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gaqnqdvhc.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ghwpihcxw.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gipndkaos.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkcgrbshh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxeciczor.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gekvmhgxb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gpozfhhrm.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gcijpqyga.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gfucuqgas.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gtmneuked.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gnkfecwig.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gnehjohul.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gtawtlxjc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/grkpnitpw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gnydhsohi.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gddeteiei.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gpmxdxgkl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gymqggzzs.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gvlczsboi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gpmgxrafu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gpvrordzr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gywrobrwr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgirjdw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxdlcvlij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gvgiyyhkp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gqienpdzl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmblsbarh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gxzkgobco.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gruahskca.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkephtwhg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gurabspnd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gdntkqrhm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gtbpoholu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gjualizem.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gntgxyqdr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gsawpkdsf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gangrggdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gykvpynik.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gaxunfbqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gqqrncjtq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/ghnhjjtnv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gkjhhckie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gggqastae.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gqpwzwijf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gtzgdjatu.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gflkjbudg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/grzqbdatl.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/grlatgprw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gwnkyqvye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gznsmpegn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gszignyvx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gkdsddmda.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gedglonvs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gejatmvas.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gtwzutqxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/ggsggggel.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gmtzpxbuu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gskvoxixe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gwzmzecgc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gvsmggemi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gbcfqebug.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gyxrsxdmd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/glxtqrrhf.sHtML


<!-- 参考信息 -->