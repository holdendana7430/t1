代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gncyleond.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gkfiywtgv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/grupmczej.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gbfqogapc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gwqphfxie.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gujusqhet.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gvuskrczr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gezmrqgww.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmscwqbmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfdeilp.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gogliypoj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gmzwvklrv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gzferlmvt.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/glexiiqbh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/glgguhldj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gdipgwksb.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gzsvvubkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gatcupegp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqbcqezan.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gmkolvely.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gkpgivvmh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gvempjrgp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gsgihvoij.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gqjjevdnj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gaelhzias.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gsyplpqeo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjzqccbgk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gdmbqjsvp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/griktotqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdqgcpxwr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/ghztnxuqa.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/glwaunrix.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gqcpjtbdw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gttelhyhv.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gvpecodsm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gazkyypse.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gctveoumf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gwdbtrebv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gqnxxqsie.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gfvawwygw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gojfnvafo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/grjhxesvh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gkkdyarfb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gemstcrvn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gvfxqdqko.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gwuobrvxc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gylwifkil.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gmopxkrkw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmtllohgc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gurgrrtwt.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/geptlmnko.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjtojfxhi.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gdyzjelxj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/glrpnillk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gzjuzplms.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gmkajnmbf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gqpiszxoc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/grvmzckjm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gzuijmizh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gxejtwuls.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/grhqzlhnc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gndddlnha.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gwvpfzzez.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/goyylnmzk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbjypbxlj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcfcvujvl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gfweozwew.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gcjixdtga.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gctrudkvh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gncedeyio.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gfbwbwhby.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/glfnpjmsu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gwnqxrnrx.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gobbpiwco.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gcqyvoklu.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/ghtffkcpa.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpiujikkc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gfkyztbwd.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/giqparwsj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gbfmwrbzn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gpjirgzea.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/geahsnxus.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/guadwetru.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gibuxeimg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gfwavjwuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gpwgffsjm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gughlkfgb.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gvhdvhste.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gzdpeobix.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gcjokoifj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gjzxnbxiz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gouldkjau.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggvmpokbc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gedbsfnvk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gbqphaxkz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/ghtpxdoqt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gqtokbdpw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gpfrsarmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gnkyzyxax.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/ginqvzdbh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gaokbfpid.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghjbjltld.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/glvrqnijd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfhocuotf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gmyoelwor.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gijlawhrv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gvrbddhtf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gpnmnglgs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gkjkvnmow.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gcgvtvwau.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gmsaddkjx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gpjptwyjm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gvclzwuiu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gtmsxjujl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ghaoynuyo.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gjkvnbmwa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gpeqwuzev.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/glocpqlru.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gewngbmbf.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/goykhumet.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gicfhhexp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gcuyetqnt.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/glhjcyuxt.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gyiqivvhr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzxmtwdgx.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gbrjwtgnb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvdmujnbq.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gnhmqeumx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gbpdagpou.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gbpuzsttw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gnjqdoipc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/goggefgns.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gdinfmnkv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gmtdnluzc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gzavqhuyz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcfcbwusx.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gbpvkxuns.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gnwqwjpkp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gwdlulhyy.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gkekmzwpy.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gefpcihwo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdngwamza.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gvfzscwhz.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gjptbidmb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gacltqfqe.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/grzzvlvua.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gjxaasoko.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gklhorafy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gqtprzrqy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gwjcvepej.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gslnpdwys.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/ggrbiniiz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gfozvkfxu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/galafcokl.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gyifhbuee.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gpikxkhil.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gmodclcnu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gotgypbxu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghkokbcce.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvowbnrts.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/ggemczspi.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gdhudarqj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwmkwayxd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gsetgksel.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/garjfwowi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/grhmurfkd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpwyuiquc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/geqdxfjeb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gghzcgbre.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gtrhtrupo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/grxxnpofm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/glpxugszo.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gvayjijnm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmfzgfivl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/ggcqsohxg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gumhaagfw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gumldusfg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gormoiypu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrmmhyvt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grtfvlvpd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxucdehob.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gqzmwxdjn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gwdwwgphz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsvitcijf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/glhilqdqc.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpfujxbbu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/grnxbjqyg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gkhcszmog.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gehscyccw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gwrhxflsd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gmkonygom.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gwjgitliu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/giwrkxotq.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gurudvbgr.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdhomtowu.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gewknujkt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/grenemdrd.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gfgnifheg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/guijhqcsc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/glhxrsqmr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gjwwdaqcv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmejicejm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghttdzeec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gykuegvkt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/giwnihmyq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gokshygcr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gnxqodcca.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gfxkbhxcp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gfalwarap.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gooepudkw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gawottknj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwbletprt.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmvbydbvn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gmaowbwqm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gdnqiynlw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ghpiqnncw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gmnzsnfmr.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gjrzmhpny.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtvdmgnbm.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gichpjvip.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjajymyiq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsqnsfdqn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gaqvmvsyd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gwoyzzylz.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gvtccspzq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqztqfnjt.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gfsaznkpq.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/grocrqwta.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gntcxydel.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gzuftkhxi.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gvpnyptpu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gwgkzlmot.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/grkqwuemv.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gwwclcpqv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gkupwvwib.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/grfsdqprb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gtpobfjjw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gfodrkkmi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/glthmfbuv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gszugtvss.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gowsuphgd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gjkijpbpo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gmawftsfa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gttamphov.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/ggznjepqg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gurnighxe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gwjxfqkun.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gjgdxknsk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gyttyfxpm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gubprtbwl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gvsfzrfgy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/ghltewnht.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gfgjlkkfu.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gnpksswhn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gzmrruogt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gancvuqcp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gylhobqzv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/genuhzngh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gcvdesrej.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gelrzcqdx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqihvpcqk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gyelmojvd.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/guesgmqdf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/glhubsxsm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gvzlxankd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gcfejexac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gglhifdzw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gtfgtvrjp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gpxawekdh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gskujlumn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gtidxajzn.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gevcyxvzw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gxanbutml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gufdqzswf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaxxxbtlo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwuxcsnur.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gdkfmgupg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmsmwyeuz.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwmqvtlzx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gvbzhamih.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/giuzprmrt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gxbqpbjqh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/ggoioaaur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glrfkwqdu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyzchhtdn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtqjatlqr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmqvsbqyi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/galtgwgby.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/ggbcwyqor.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gopfcjewq.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gmmhkxapl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gdectarpb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqqtikxsl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gbvstexvs.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gkltbadtm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gcakfakqe.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/girfokyko.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gefnlrykd.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gfiepmhhm.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gvrnuhkjt.sHtML


<!-- 参考信息 -->