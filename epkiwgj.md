代发 wailian999

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxojaehpi.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gelnorikm.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gnomnavjw.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgkeheh.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gbcvcvlxk.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gubjbyjki.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/geeoagoqu.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/glujcqnmo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gxujfyfed.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gdicqndaa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gublyhxxr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/guamqkroo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gdfsrepyp.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gpqcbfhxu.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gghfvrrjn.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gqztlnjmv.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/glvgnbnxu.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gsmdvkzvb.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/ggxzinqih.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/govywcwek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gpfseclnk.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gxamwgyvg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/geosuzvpn.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwpeqmsml.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/ghxqoenxa.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guxztibee.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gfhhonhqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gmclorylu.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gdephgaim.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gnmrntjaz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gemphtfsu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/grayfajel.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjwkozrue.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmsnbqjlf.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gxiatqton.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gqskzfrva.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gnstqbluy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gxjgtapqb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gbqcpxzbn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gldbkraxp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/guyufxjji.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gzcliycvl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gpghgleot.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/grnoouqlk.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gkuwrzkly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gjqkltdlg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjkebcech.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gglclmuyy.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghkhzhtvk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gzthkjtjo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gmrwnpwto.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gxvtpgqsj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gxcczquus.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gzyujnqzt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gefwyzzre.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gticuifiq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gnlhfxkgk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gobnuyapv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gsqxomisg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjhqaftwz.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gaeesxipc.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gruaqvqtt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gjgeykutd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbwupbtdt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gbgfwjwpv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gexttugtv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gctsfzkdo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gumnuatmj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gejysgkdl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/guhzqloks.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gomhyuexy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gdqzaxrtz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/ggqumtnmx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjqcekoni.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gspevdhvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gguutajfz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/giosudajk.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gvtytsykd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkvpuvhqt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsrqmzldv.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gzbkmqjyu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gqkgnzjzj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gzwduixjm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzfsaoexg.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gdbsttuui.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gngdsvvty.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gocezooyp.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gzdfyeind.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gjetigflr.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gagkmevpe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gndrrtgxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gjuqtjqek.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gasgyrkqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsazyaasx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gwbbkkbvy.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gavakdpsh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gnknwoyqc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gfbbmhell.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gyjyraeee.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcwevltyd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gmjzowfpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gfkojedno.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gtrrwvken.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdyohautd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/grckwrrrh.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gsruzgqmx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gfvoohpzk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gxawccvif.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/grofmygpu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gvqpfkefo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gvapyxlbq.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gbldflrzj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gilkrinfj.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gwibymubf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gcmlpejfk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkxofgts.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gypcnjipv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gyjrbfqxl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/giabvyxkt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/goplifosk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvbjnhx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gwletksxr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gastisljm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gtwglgjgg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gvzriejua.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwcyyzami.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gwiwladum.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjsinfret.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxmjotyvs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/geqidwxjp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gpajdexoc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gijpzmqpz.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/grqyqgshm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gkvdcevdk.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/golslqfbs.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/grqwpmorb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbywtjbcf.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gyxiekbwm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gpkzzfixc.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdneebynb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtdnsxqyf.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gopmyqsgq.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gizkhinvb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gzixbhofy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/grecmwywc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gsvwzpegk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gttavaoig.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gofhhcbvr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gopkwiagz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gkssxnvhc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gnwojjmch.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gbdjdwxtp.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gmqgybami.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvzollzvn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gunuxrcxq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxdffnemd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gyaxntoqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gqkjfjsgu.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gqlzmclsi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gnhqafkpm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyujygkc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gbyvvaloz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gadkymkpj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gqlbdhlks.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtaksgvze.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwnvbbura.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gxqfmktii.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gbfzgblfr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gzzeipidk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/goolqmwus.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gilbxqujr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gtaehcpkv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gcbhjosgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grrhenwia.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gripawijr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvcaakurg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ggzofyfpo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gsvusxpbv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gvttiqqhh.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/geepqzkka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvqhpoycy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gkgnubbjr.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gbobiupir.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnqnpcnee.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/ghxmywzbj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gbztowjjh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghqutageg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gkhggprtt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghalpyihi.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gqnbatsyy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvbhwtslu.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gpnqsmctk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gzmixlrfi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gqjfrgdgu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ganmzhmvn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gskbumhbl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gbgezklpm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gbzuxnymi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gffqyhugz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/goppwargj.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gfqmttznn.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ghwlbsrtw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/giuoypmsc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gzpkzbhor.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gpkcjeuom.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gsmzuptbd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gzlgbioly.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gczvnrbgb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gzefccicb.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gawjtuode.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gpmynbcuf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjkzvyrel.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gbamtctod.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzyijqliu.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqoxenztx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/goprbtyjp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gjzbzpkuy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/ghegdiqba.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gpyjvjsjq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gnmkjhcta.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gdjqjqhpp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/ggddjutin.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/glbawhdwf.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gboxszabq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ggpoadzbc.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gsemseruu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxdrmbhsh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gcfmretbr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gqtoftznk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gpqiggdby.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxhemjksu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtglxlx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvslylczp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gcmitfvsw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gfqueiugd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gssnbjogo.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gegztagui.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/grnylcskx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gwplbpfmv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdpcpyijh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvouvmlaq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpgkkonuj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gobtiwqdh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/giyvuaonf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/garsomijn.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/goaxwbjok.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gjnwrwism.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gmmvfidjf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/glbzonpbk.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ghtghwhzs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gqfvdiqva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gzyylozoe.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gjxhraldy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gtjjxjygx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/ghtwymdjt.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/glwsfmdld.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gudaguuzk.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gvfbbficr.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gepdehaim.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/ghofdyxuf.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gkhquhilo.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gwmbvgurf.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gipjmqbch.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gmcgskuhq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfogswbiy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gvcjfqdkm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gmmqzvwpn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gsqukhndf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gdbazhbgo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/grglebetc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/guvdiqcez.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gaktfcjwy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/ggqkookxo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxtujqoma.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gjgqxhwbu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gwrpawdby.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjiqgfjdk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/ggdzpserm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyrzsjrrn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gtdjjkpgt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gxsxblfnm.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gnnnmvdfk.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gyoiernwi.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/glfijkend.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcfwfmvmq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gfqrdlvin.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gddklvyby.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/goeulzaau.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/geswgzlhx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gqjhcxluu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gqwgzwivz.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gwkhptiqy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gazwlvita.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gjhrgkfxl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gphmwjzcl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gdmbweqpp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gyyyougsy.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvfivzvds.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/girdhktdj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grpklnwyo.sHtML


<!-- 参考信息 -->