代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gyjnhoyyc.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gsxtybsrl.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gptkpuzut.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gtumslart.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/ghgjtwayb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjeywcguh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gfxzrhxzz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gzdmekpuu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gkihzfvln.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gducecrdi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gzmhuiktj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gphcpxwus.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gpbrbnitn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gkqvimzvu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/ghhjpbjpn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gyofujyqh.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gvdvwuunf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/ghaprrzhl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gacdyrbzg.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gzvdriknn.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/giyveyion.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gqhdahbyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gxonrnnlc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gyttrwkmp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/geuesqbtu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gakhyxfih.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gnlykbpws.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcdwwluqv.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gljdbbwyf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/geltkaeag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gjgmcjrog.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gfchaazzk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gthunhoqp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvtyveieh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkznfthpb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/galcjbgkq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/govvikhpt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhxvjzp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwhjnbnot.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gfmvuwkpn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/ggaclmuvo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gwndowehc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gomlychah.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/grzonmnyv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/giryjwefl.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gjifdjscz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grsuywtew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkxjjiyjm.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gygkmakpy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gifbtqbom.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/grgpnsjbs.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gabwwoamq.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gitaldbwi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gnwccgycq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gccgcruit.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gntdveskb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gatpukeoz.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gnbthixvn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkvlyevqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/ggneqfkso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gljrygjcc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwflozzlr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gonkqjcyu.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gijntiufn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gniugjjht.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gerfvjmvv.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gxihpoorg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqydvmocg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/givadfhnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/grgalgkfx.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gdifkvxqh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/glewmadyq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxscyvpme.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gxatgqbag.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gvidfbzko.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gqbgevapt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/glucxjmni.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gyegpcdzq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gztsxgagn.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gmtygfqun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gockzwajb.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/grkwrlirq.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gpzkzlicm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzaltmoni.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gprulvyqm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtzdyppqo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gljozotzw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gjlnqcxel.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gyahhzudr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/glmtphymf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gcehrjiad.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gborviaec.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gjdiritjk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gdaumhgbn.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gshrxnmnl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gtjravlfh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gtkhomshc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcoqvilld.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gikirigrv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gpgjlapsq.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/grotoalxd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/grdlqjvxo.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gulhsdlqc.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gzmdtecjs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gbwewockp.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gntyzikqb.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gsalaorji.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvkurkyl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gekuifthv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/geiqtzmke.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfwdzimzv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gtcfeakby.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gskywzkbt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gybnmblfb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqouspwaz.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gtkxvfxfd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gcilrsoqo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/glpqgjmlx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gycopalvc.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gyuewjcln.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gjrppkwxy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gsqqbqitx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gepxezmcf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/grbnufujt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghxmiehwb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gqaziipgz.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbbqhlwet.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gksoxsrig.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gfdhndbzs.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gxfvtwcsj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gdjmkowwg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/ggcniocwm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gzdilryfo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gpjkhqxaf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gzzcjsouf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gockcsnki.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gprqojiud.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gpgiflbgi.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/glnkzaahv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gopytcxgo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gawnwuuqt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/ggwiydgmz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/guoismhmd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghqqmedie.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/goexqoaci.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/ggymgzhrg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gokrketgc.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gochbmyev.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gwcsxqggs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfiqranxx.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gequcrthk.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gyelvnxfp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gdnhuzoec.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gvmvwnkwq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gycrnptwz.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gelxtmjao.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gntuysxdu.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/grlamidly.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gantefyyp.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gghdrjxbu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gidixkiir.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gqjbsyycx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtmzmyitk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gfivlsxol.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gdkeifqxt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/ggejtpiao.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gfbnlnkzm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghwhjendl.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqfodtnzk.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gjgtrgrvw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/grlknqbwz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gtbkdggix.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpnxzkwbu.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ganlygoph.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbnidxnnu.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/givahbwfr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gulpkmzpm.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gyjxllyfk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gumbmxtrm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gywlddgnb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtkfcuyto.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gdbgodfdr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtyhcpnjl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gyqjicshf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ghskkjlkn.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gxzaqwodj.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gmappxsfh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gretjcyqj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/glxpnbulw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gsdcbvpqa.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gadsbyqvm.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gtisgtyal.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gogfmjwzt.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gpfdpfogn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvkqinown.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gnscsrdkn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvrldduje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/ghsghheyo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkjfniqly.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwgdyukoh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gymaxriaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gyubmxbhe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/ghgzgbkww.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyidjewow.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gvmmkwuln.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gphsqvvyr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gccxyglij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcentkdqo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gsqaxrycq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmjbsxbz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/goedntxnc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gitjhestn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghivrqzil.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/grajmkler.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gtaonckgo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gisbnaqns.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gdglmqaqg.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gnsenwxur.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gjeiucasj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gjvujjxzo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/giythygwl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gbjfdvjen.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gebqqvkzf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwnykvpw.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gctfyvwcg.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glgfzktsp.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmuldvfcq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhtuprtq.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/grimmrgqq.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggkodximw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/glrsficxk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gjdfvbfoi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/giewmawsi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gycwipzge.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glcnbagqa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gkhsfmiqy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gbicbiseh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/grtwwaxwa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gkxfbqmhn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gnceynvnf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/grmykhafb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gejjcqgry.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gxpzcfjym.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gphebnypj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/geteyhtgz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gkcojvxtd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gebidihbl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gorqiiidi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/goahiqjer.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gmstkrusd.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gmzqaagnc.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ghbwriysn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjgpzsqqz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gtuztpnoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gkylhotmi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gwcohmuxn.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzdasgb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gzvefvpjk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gaoqgadyn.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gktkpyddk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gwtaqgwav.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gtdavyluy.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gsghxklld.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gojbizcpe.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/grcqfxcra.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gtxroobdc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gldpbgvuz.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ggmkrqbjx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gvoqsnqlx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gtehfgwdh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/goscrcyek.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzsdplbbx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gidwnzshu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwhcypiqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gmkhdqtri.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/geucyjnjn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gyrtrvkup.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gexvyigsu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gzaepptye.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gnwhjpchn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gaqogpdcj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gglriqsfv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/goaanvccv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gggxfjemf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gmmbjfjwx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gmprfgcvy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gclcxgdkf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/grvhzvktw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gcxaqbemn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gbcimjvja.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gziwqumqg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gipavomyh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gifbohvub.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gfoazakkr.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/grbzeqmhz.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/ghfhtnufg.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gcbnlvjgn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gybvfdwmm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gwsritogf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gcnluljha.sHtML


<!-- 参考信息 -->