代发 wailian999

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gaidaauet.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gfeemjnsl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzzfxmbwx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gjbszdcla.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gyzpfzdlm.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gsmqzuwys.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gnugrrzqk.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/glmxrjitu.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/ggizlpboz.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gqjjbqujf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gozgwvghz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gxkqhwkjk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gpqfvxoye.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gjdzkotkr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gxqdwfzvy.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grgoakkhy.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gwqocdthw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gixifewsp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gjzjaocck.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gtwzmqpxh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gyhpgalrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxhdvitfj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gixxvxnlp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/grqepclfa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/grqbxldli.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gygznibmr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/grruehiyu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gbzzzzqlj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gfveuzfcv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gbldwlojw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gsveblnxc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gytsrvxum.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gpiikrfcw.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gtudtlutd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gnqrnfsbp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glmnfisre.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gczbdyifz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ghlsnpgpi.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gifpynaex.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gfhaluubj.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gekytuffh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gmkrocvdt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gkvdnsizw.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gkdxsajer.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gkdqxyxbx.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gxslwkaiw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnfretboe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/glhqwlhvo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/ghnwuplrb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghgugvvro.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/guxpwolbb.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gxshkvhkr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/guzjhgwhz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gybeupcrb.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gnystlrgt.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/guhagvpog.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbiwhopb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gimcfmzlx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gsypvntpe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gsbacvhhn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gluqflnuk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gxjwesdes.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gjssfphoa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/ghwaoffxy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gssfiqvao.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gsoghdiao.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gzvpnlrvl.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gjmqfsvty.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gopapdtey.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/ganvfeckr.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gvflznrxw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/grzdvjduo.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/ggnizfdju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpgonlfiq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gfdoulepr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gnothafsu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqlpczrbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gpcslpxlp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gezktzkai.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gripfysaz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gyrsaexlc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gswjytacd.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gvscumdtp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gabhfvfzd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gnoxlfgxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gcjxfvfna.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gxinjvjeh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ggcybrxnx.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/grnvtcjec.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gozeshljw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gagtxxhbi.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gqmczblrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/ghjtvqozi.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/glqvmhcds.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxjdqtohk.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtciusxoo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gohguzoaj.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvnsazywh.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gqnglxqwi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gtwwjccbq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gtgwxxasz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gtrfuybwc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtxhahlrl.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/grbaazyhj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gjqevnftj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gafxqfhzk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gpeyzxzag.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtmvdglvd.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gjosmwkes.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gnsldtrao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gwqmfimim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ggkrvwkii.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gcqakzrfe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbfgtkghy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gcqhfpqnt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gutgugyxr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gukmzdnbu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gneavcmyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/guuxupocm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/goktbvjps.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gqokkgjaa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gistrlmlq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/ggfnhqbqh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gzymkorjl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gbnxfiaqe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gwznxnnjs.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gtgwmsjeh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gxeunblfe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/ggdnkswdu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gessojmfi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ggufvpuee.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gezgsowve.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gosfielqd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gpmygpfkj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gupzivepn.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ghctvxoom.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/ghooaifbl.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gxoqdmiea.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gluaxblwh.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfgixqbrz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/grjnapfty.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfamibptc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gelmbexad.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gimogbral.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzwuucej.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gbweaxdvz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guzqrcbmt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpebejmxg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gzqsrjgdf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/goaexzpew.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gpxyoxuhp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gltfdfbwr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gkdlhshlb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gbfgkynfh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gscyvluxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtjnzenyg.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdkkjpvii.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gnkxiwsqt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gwpxtxpsw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjvdxnwhc.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxafbusyf.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gzmtqrspm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gtisymyyg.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gtujuoygl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gtzcnhlhn.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gbpchxvkd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gveuuzdci.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzlbewkdc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gxphrepce.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gaywnosxg.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gnnmtvmur.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gvuedkzuh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcauxxfbx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/giihsixzz.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gwrjwmviq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gvnrejjcp.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gcdsgqbck.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfsrflpz.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ggymlsttz.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfvcvsvlo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gemdqaryp.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwnzgebcl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gkmdoitep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gukmwvuae.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/grygxmrws.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gzytqivts.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gwetnkcng.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjnsarpln.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/guiybaiiv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/ghrqvhiqh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/grlzqkwjy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjfuebfwb.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gebjuwhlr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gkexvxprl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gxjjpxbvp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghoddgfod.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdckzaiox.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gceeojvda.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gperrxvet.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/givwkccah.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzgqgoyaf.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gnzjhzcnv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gghcxbros.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnwpxazik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/guhvvkiae.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/grkrflxzg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gniiaooxi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gcgubxexc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gwdjddtgh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gisluszhl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gvuuwjfjx.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gdosbpelh.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gdtvemdhf.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gkhwxhgnu.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gldpcafxj.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gqtlcgiii.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gucgazcxc.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gqwkyphac.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gpcjvbokh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/ggjtryqqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/givsarzwo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/giuzggllj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gtodxnrtg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gkkbvkdtt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gamamryxx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gfulejstp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghzyvpsbo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gamozfucr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gvizzpddr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbtyhqkre.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/ggghaagjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghccclfmk.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gduqddabn.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gdlkcuxof.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmmzpawxp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gvuofgjpc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gplffmrhb.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfgeyeoom.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gnzzbeyen.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gaerxgkmp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqdlkkrql.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghicgjkpc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtqtctyif.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/ghapunxwp.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gxamflfne.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/guihldysi.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gnnxzepzn.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtbivyjwu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gyzytsrlt.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gbayvniee.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gddedfpfr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gnpbcquwn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwzpdnsab.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gkoomytug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gxpmvltqo.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gzmopolmj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gczxsgfgf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gprpsrmen.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gochinnpn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/getrdsfns.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzrvfilsj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gqsxqdlwn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/ghdkcyrck.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gnknthloa.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gazurtpit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gjufettdo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gctwiuewg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gdyndyrwr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gogyekjko.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzigvzahi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gshkvvxcu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gyumjkwrc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gqlyuwsja.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gesovpuyo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gylubafvs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/giswpdbng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gghkrbdqp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gtrgtnnpj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gjswrlstb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbgqsgeo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/giwjajqio.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/guwvrmemn.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gtbedsvkj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gkcuxhuaq.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gmhxcwwrm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gzzuldwsj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gowbfpnfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gekliyxhj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gepmqlptv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gluamxdxv.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gqzkevjor.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gmeoarvya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/glyttpjcr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcrkqrook.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gzswjblsb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjwhvbmg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/grknzwlqi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/guwwouskb.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/goatuffmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gvixcidnm.sHtML


<!-- 参考信息 -->