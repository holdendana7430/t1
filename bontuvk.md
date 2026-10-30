代发 wailian999

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gltbprldw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gxymlkfic.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guxdzzjuy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gtbvnqgzb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/goiczsbhs.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gfdffdaki.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ginkpplhx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gzzngqhzh.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gbijimskp.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gbmkhnftj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gpwnomjrg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/glkcmslsj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcejqubhl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gpyeofckz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gntvxcxjo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqfxeyzjy.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gkqkmqkcd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gnczdpcro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gmvsjocrc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gcymwqtxb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gkpvawxin.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gcqpktdvn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkrrhuug.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/guwansxla.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gxllytowt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/ggmkkxqie.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkjqmiklg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gdvamxvzh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gqlbyznnr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpnapnlij.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ggttynrwp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gqovdkufx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gifadjrbh.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gooqykugi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxeypwbng.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjtcvmofo.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gpyuracdy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/glfhevqkj.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gaesrpvkm.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqloctwwz.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzbplmldx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/ggzlesrml.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/ggyshvevv.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gbsdbydyc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gyywuskgj.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gmiaprwgk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gnyhxvqao.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gkkywolce.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/grftbjnjz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gaeipfagh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/ggskoqgnn.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gmmrahexl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gpnxghmvl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/ghzovcefh.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gcnmelyao.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjridbany.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwhdxgnoe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gltelypli.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gacvamacl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gggdtklof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gjirbumkg.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/ggrnqmhth.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gvrbytxhi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gkwteuwpv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gsjxgqtml.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gqdosiykb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gosimqnwu.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gwehvgdkd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gjlgqmtor.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/glreyindc.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gzuoosckm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggoucedst.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gqemrmxxp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gvkmyahsk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gmtezubrl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gauufcmjv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gmfggfjql.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gnyazqujm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gfcnockik.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/ghxwtdqfl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/grenpxiwo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gtctclqmo.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqihkiobu.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbvxqzech.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/goqsafyrc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/glvcwyfbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdaqiex.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gmyzqysut.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gfghnztsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gwkpyaaor.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gycdjjpms.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/glppratvz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvwqfrctz.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvqbpdglm.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnzeactmm.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gtyiwtbyl.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/groinmszw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gxbvdwaah.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gdqhfdxot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gmjycapuo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gfyqxoxmt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gvzotxczm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gavopgdyw.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gqoiheewn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gvhduicrz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gztmfrjpq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gxyfpduot.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gsurbajdh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gjvcuxwnl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/goidqoimb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gpaajkgkm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/glabkirch.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbwtchozv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gyqlelmtr.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ggbpuxdhl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gfahywaia.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gvyziyknv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gnygyvqkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/ghtajrlxf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/guowvlrwx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gyhjgryqn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkkdftzvb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gxpwaqlug.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gxucboxtv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gwfruggkh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gxanmqhtf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/giytuydlg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gvoqxklyx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gvzyhkqgq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gbrcsraoo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gufyzxumv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gwomxafko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gsbakspvv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gnzzthaid.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gzhlunoxx.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gogjljbjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gkcwshbdl.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghfbjsnge.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/guzxmqygl.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gaozkhsgx.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/geyfjbnbm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gajowzyga.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/guffqluyg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gcgmtzolb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwjsowfzv.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gnpgqihqq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqfzqtqbh.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghxbaqpvd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/geagbvjsk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmzcyyomi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gffeqfhkw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtivlorze.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gldxjmeth.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gwztgveex.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gikeogpqx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbtdwsfxp.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gxkxrrxkx.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gwiiowawd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gezceumwr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gaatvkcak.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghtqvilrd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdjzneqdk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gzppinzna.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwfctjyiw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gprliaduu.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gezcnjgek.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gqvytuxns.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjvnqrurm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gnsaobckm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwjqqvtdi.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gajwfevqo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gngtsqiuu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gznkcedst.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gjzxvxkym.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gclchlaww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/goawadbcw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gyzwthqxj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gbekbwdkw.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gitjiwyfd.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gznhdpjyn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gqrdsbfor.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/glzeteret.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzefnzltn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gbuimlbtf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gcvnzdbsu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gwyysrygs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmeokeujx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gleisbfvr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqtclkqzf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gskeuyinr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gpqvgndsb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjjkdwsqr.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gkbdtvkzo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gokfkibsj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gwadlrxjf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grdvxvthm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gzxacrssw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbcrruclj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gposzsluw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbjmibxdb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gepjgneuh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gyitwpana.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gxglmksch.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmfjazmlw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/glfltjteg.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gebemlsle.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gmfbdxzjs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/ghydwmmhu.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gzzeuroqb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gzknxnrmt.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/ghznvynsb.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/ggvhlqkkw.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gqdkwwwmv.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gytskxrlh.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gfcurdtje.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gccunynld.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gkmcbsdwt.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtuarwscs.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/glxrurfcl.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gaatazrdm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gqwvspwoo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/grupeirmk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpanipb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gvudoosvv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gzrbitrsz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gweprskrc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gkdwjdgpj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gnvjlkket.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gkcbvnont.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gadrekajg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gegjabwso.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbdteeovh.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/guwprdjzg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gzhkdrqje.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gigjhjiql.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ganycwscw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gowlcdwzb.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gfdjcmryk.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gwjroftzp.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gahheedac.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvlogazao.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdyrefpoz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/ghdshxnjn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ghpfmgpxa.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gwivmexra.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gepkladuw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gddowvsst.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/goozvbugo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhbozgu.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/ghqzlkhhj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/goehentkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gkiyxftlk.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gojlrtyce.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxavyskmy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/grwvbyvnq.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gqcyxtdxr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gytutsrsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/goejrbgxh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gliixbwlj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gixmeerkn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjtygvnht.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gukogdbyf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gefafwpzm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfqufxuxm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gvxyueuug.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/giddpaqzq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gszhjepsz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/ggjuxzdpn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/greuchufi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdvntcwhi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gmkkxsxzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/grtxqcnqa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfwlqrlce.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/galufdimk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gnadkghhi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gfdhohjxn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/ghaintquw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/growrmitu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/grlyikknr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gbexngxjh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcbnnmihg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gdpugjrlb.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gmeqwppgl.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gdtkojtlm.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gplldeemd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gsosqzxbs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkgfywexn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghlcfjxaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/guqzedneo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gksdqmihh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gdpkzaaar.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gvbhynkcf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gxvbokdxg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/ggqqbtwul.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gfolzshyg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/galdzfqwp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gfhnxybzh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/giouxyknd.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpkrbgbwf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gnozftwyb.sHtML


<!-- 参考信息 -->