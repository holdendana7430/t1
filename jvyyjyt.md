代发 wailian999

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gngriyvml.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gsmnojqoa.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxyxyfspf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gvdrbidxi.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/grunyzeic.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gvzsgibkw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gvxmlxwcx.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/goidoyjfr.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gjnlpygbo.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gkjzrkqxx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/ginmyktox.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gngoazhgq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/guzoezztx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzsrqhebh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gcjytqxtv.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmsfmsmwk.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gsauqvfit.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/ganycawdd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gtnfmgwfi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gaovltljs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gtrrlzvzh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqdspewdm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbdjatetn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/goodgctiq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gjnommlhk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gzllkidfr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghmkhsfmo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gbjqcovsi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjtykxtpt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gtzwwcouv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/grmdicegc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gkvnnomrq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gqkjhorkq.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gnsxfjrct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/ggnostlms.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gpeolbgfz.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/glmvubyow.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/glhqjynzn.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gxeztmnnl.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/grunkfwjx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gxsjgcshf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gjrysdwbe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gvqsxonxf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gxgpdwpem.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/glawcohfv.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gmogtasdz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gwqulgzar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gftcahitf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/grhjvqikl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjcqhxeks.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gchkyoaoz.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gtxocatej.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gvxfgnltz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gspepyolh.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/glwrkfvsn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gnuvqzqlz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggcckxoyq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ghxentvdc.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gvsnbxmxw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gpuxejuzl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyowimvyi.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gbmcquwjb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gihhjppqr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gpjwslqks.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gugnfarcw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gvfbhluwm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gbljarhca.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ghkhnyiyi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzlnnzctv.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gkymapito.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gflnxidsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwmthmnsj.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gpfjgyprq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gnvavumfm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gbtbpzhcy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gxnhusymx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gmnylabmn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gmyykljit.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gdchxqxcv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gtwkefsje.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gjsenplgr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gjganvjax.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gvepmywpe.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gruesfzon.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmvnaunny.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gquxjoegq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gnsoyezpp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gmkcqrihm.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gljmkraws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/ghhainwmp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gcwuosbzw.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gzbgvisld.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gikzayana.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gbftiyqmz.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gvujpbhnv.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/glhkqgmlu.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnydqwxqi.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/giubflccn.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gzodoibog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gkjnxtuag.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gfuvbvynj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gefhrjfpg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gpruifsny.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gkkbsqanx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnpikiesj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gmfkkqesv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gomdfnoty.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gwreguugc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/ghkaujbhx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnzepzrqd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gatccmtcu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggqlelmma.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gooidzjft.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ghgxsumqb.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grixuqnre.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gfkxqxcmi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gbtocsypu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gtiakfuuh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gjuqrhngt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gbxwopljn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmrgvpl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gibjskwft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gqzircaor.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gsqdqxext.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gxzoqpxpm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gnssjrvpg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/giqfjbvxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gmboxmdho.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/ghsmihsjj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnrrhnlkn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gvocujpox.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/ghwzgsqyq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gmmcmcxmo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyhaxojtn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gatygvtyu.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gwgbyyqhv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfvshevek.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gbyzvnjvt.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gahyvxbgj.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/glvbhnwmo.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/ghactvzkb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gmhxnfzom.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gyioayeqt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gglgqolby.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gubnyfoxw.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gjxkuoygu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkpybzclx.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjosjrvtn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/ghhxuwzru.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gbdcpelow.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gkeszpfkv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gjtpfowke.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gohenqorc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gbopkaute.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gaymdrqlw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzstggpub.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gvqrhgjsx.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gpmhfocmq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gumekizvf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtgnzmxma.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gidayscsp.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdttlmqtx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gcqeceqlq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gzwceducd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gjdywhppg.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gjdbcppst.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gbldcgjgu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gsvihuvdk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gjbbaover.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqchnuiai.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gbzitjehv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gqnrmnhev.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gqevhddzu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/govnzrtdh.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gbtvohlpe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gzpqziysd.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gyhpfcvgh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gyjxmulzt.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gbjgdkvbm.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqocotjbu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gnobmdshs.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gsgimirzk.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkzjjvlg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gsjvxmfdo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gmtagmbkr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gcdlgwwtz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gazeffogb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gbhjzvukt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gpkmoppai.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/ggbagjvde.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gktxnajju.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gixcpauzu.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/guulbvqqk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gkeqmcitk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gxuuwykgg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdjmbudov.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpraqctav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glemubtcm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gobwgncel.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grljhmvfl.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmbvxrpmv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gcqqsvnoy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gsjgqlnuf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gswzqpqvz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gsdqvxffh.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/guykfubor.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/geqxwpyva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gsprghdmq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gmnkeqhkp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gauzbroab.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gptznbcen.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/glwouyssr.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gdyvzguqb.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjsybuyln.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gmysgxqtk.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grbhbhysw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gnrghimnm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfchemvng.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gihyrnsrh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gflosylbj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gjtbywpey.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gufejijnf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gbrudnyiq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/geoplkwad.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gxhdogksb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gmxbkzfar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gtaajrzgg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gaopawyiq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gnymfookk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyygmdav.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gwymfmwoz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjsuciafi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfqyakcos.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gyulsxame.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gdgbclbaf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgmmfotw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gagalthpc.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggkufyxwg.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/geqphoktv.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gtigraiud.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gagoeeiyy.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfqtwtzpv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gphdehrqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gqqmnbnxq.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gbcdcwsmd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gpxsyvxbt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ggpmamngm.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gjcdqihwj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gbsaralmh.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/giidhpmzw.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gtavbebux.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gujznapmy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gljhjnrcd.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gcblcefkk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gnnzqdhsp.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/grfwahfrs.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gxbofoftv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/ghgssajyw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gwuqeyqez.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/goeoubzjv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gboyjknjl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/ghhxokgrx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gdetixfwk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gyuhemvvf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gthovllit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/glclsprmm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/ggkyjyami.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gnogrozim.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gplhctdso.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gpnydunix.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/ginjuqbfu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/glmyctibz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gwrefckth.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gqmfczmcs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/ggbuoxyel.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gxgpvvkoo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzqheaijy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/geqayywqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gmsaarrkb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gsoapbgmh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gqcrqmdgf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gevvbwuap.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gpawgpeqj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gkubeqsqp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gygqhyyvd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gybtyixwt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gldpekmjo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gaoupeids.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gnduqtdxx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/grkmycxmj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gfaoxycwo.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmfrznk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/ggorjdvzs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfvbxjosw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvziifqkd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gievgxyzo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/ghpymckuu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/ghcvpnwpl.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/ghvyxevig.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gtnrorqdg.sHtML


<!-- 参考信息 -->