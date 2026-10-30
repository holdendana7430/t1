代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/giercympq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gjwmppjcn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gqpgjufpm.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gvqrhpgio.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gahuawxio.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gkwnxchel.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gpwwlqnuk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gfjecjnyc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gqkrxnzdp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkmgoqddu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gvypbvwvd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkejsxado.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gvkvcruiu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gitajtdwh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gpfalnpfx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gxhtqdpna.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gccumfxin.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkuddzoe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwnjfszqx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gbdbksfzp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/givqepsow.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gdxraftrz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnotumowq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gfuugazgz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/giokyfptb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/glvpduhzs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/goztasrdb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gcprcxkdi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gedksaxac.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gxaofqdjn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/geseuzepw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxwchifoc.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gonbqaxxs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/giukthuqu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggoofzdij.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsmzjclqo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ghejydgwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gveseuixe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gmdicdfjb.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gvwgwvbwo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gbxqkvpsa.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/ghrjkwado.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gaecwwqim.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfjwtusdn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxbaqnsnz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gniaxzmjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gmghnjjmt.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gqfahsomu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gjoulvfox.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/grdomudpe.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/guencrlxb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gbcujnddx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/galrzqxzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/guvuujgpi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvhhqqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gectscbss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gntpyrlmd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gtrhvjhqe.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gxyobwokf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gplfisftl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gayrhxbcm.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gjetxznrb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gbqunhhkm.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gfcrsesmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gyurnwpcd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghmybudlp.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gvthomzmj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gxvsxkxho.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gaqdrnrgq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gjwfhodiq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gplfywunm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gxgkokmlw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gdbxqzvve.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gakcynvty.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/ggcybbovn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gohefamap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gbfctjcyq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gddjdrgdk.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gsxshdwol.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/glpugjeuj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gaezbckca.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gveynobyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gikztygcz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gzgldgrut.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gqjanqagw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/grrsrlzdr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/getlrdrit.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gevtndgxv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoijmtrt.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gvodtpkcg.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gidyykmoh.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gpjoxhgdn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvfnbviov.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpgsdahia.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkzsslshf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gjlnykxwe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gemlhwnqi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjedujwfv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gwhkiewnu.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/ginkwlttf.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gyzrpddck.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gncagxfjr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gkxtmngzf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfcnjhapm.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gxedjpjoa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gbyvugwms.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gjlzmatof.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/golwbpyxr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqcpivwgx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gibvnhhfk.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gjlqxmggt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gyyfugbtg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gpdeifntb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/ggcyezubw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gicftofil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gvahsnqdd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gjtgcvcgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gngeksebr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gskuhwhzm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gpxshrtvb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/ggkwgvmnm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gzdncnvnm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gfvpxuhwy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/ggdcdcbjp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gupctznzl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gajabicty.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gsxpxzrsa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxfeasavk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gorbdxoyb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtvithlhq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gidogrxoy.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gtzadkboi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gxqvxnmhe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfwpaenjt.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gkpzibkyx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gviupbzsq.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdjdzyetg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxanfzdll.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gpoabcamr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gxyekxhaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqumblxkd.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gawvxfarh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guwiwezxc.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gznyogzem.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gcqdairnc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gnbzjkqqu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/geoeonsye.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ginvcitdu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gbefjchjz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/glkqdchae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gjlvzbgmw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnfjiodch.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gczbyflbu.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gnbfnktik.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gklpxdfda.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gcsqtfxph.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/grqdzriwi.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gxwmnjfif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/goelktpzj.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/guhxfbmhu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gycmwmqmp.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gxoeifrmc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gzdpcifnp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkjdfiukm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gnmdldcsn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gtsugxfrp.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzguxxjzq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/girrrlliu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gtzacmzda.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gocuhhyid.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gflafkyuh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gyhuovmxc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gohutmskc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gonhhugli.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghmnkgshu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ggoihgapc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gyatfkekl.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gtzumyoxr.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gltgkjjuf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/griexppsp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gsqjoaifw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gzwafpjwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/grwmjmfas.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gvtuaiagl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gfhvdpghl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gvlltofvv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gywhyqixl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gkaxtgrln.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gyadoomot.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbeyimps.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gikdhqdvr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbxlmyphj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxfncrnvx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmsulyhkm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gspzhmnwi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gidmrdolc.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghlbuzfck.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gdsxdppfx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gmwbrinfn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glrzbvbrm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gipwjyegp.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gxycehxvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/ggwqyrxyq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gvviqowsr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gdhgawynu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gtsjnkqvw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gjnfwkycc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gmsqhwypz.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gjqtnqpyy.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjkgnre.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvnwevmum.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/geespwxfx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gghapmywq.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/goupsjwix.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gwgoubxwy.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/glksgazhd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gtnbwewsx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwtddjtcp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/grronkjfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gseovzavh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gimjelavh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/garguxxom.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gutkmyboi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/groqkavyb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/geddvvetz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gbyaarvfx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gtggygfki.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwcvqcttw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdacevljo.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/ghqiphzfu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grauvkthx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gknduqzsf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gtgqxhmpu.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gbejfxrno.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/geuackhkz.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gxdrdaewp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbixhnuqy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmybknqcf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gknavtole.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghgmubjxv.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gncnhspcu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gdmktsuyx.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gjikxurwg.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmqvronjw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gytkbryui.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gxbksylop.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gxsgptuuc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/grxzcnhtt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gkgdglbuo.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gcycyqkzs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/ggrbnuhka.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gggdsgxho.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gnlpqepyt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/glmqxrfec.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gzqmcesry.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gspkhhtfu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/grzbanqym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gldlpkayd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gogkypxqk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gytuxafnq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gmdamoagv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/guzjapjdj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/ggpiyzynp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gicxliovs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gqnuncarc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfjoyldls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gpvcfcsda.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gpydnrwln.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grmbgfqel.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gwenttibr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhrgwzbf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/geqfzesnt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkplgpqba.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gohchuxhf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gtmzznyxf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gtskflpnz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gepvkfnbn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gzquzropx.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gnxqbwjkt.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gcexryube.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gokbfxtfa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/goitsonjb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gblgvuayc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gszqdcwwd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gjvrvcljr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/guudraooc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gtbcntfpn.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gqcvbxdpv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gocldusmh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gpoarbuwx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gfiknvurc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gbdtaesre.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gmubxsejv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/giochnljh.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gygmgcizn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gaxvctbnh.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gobzqykls.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gkudwmjkn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/geyfsvwre.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjjfspnal.sHtML


<!-- 参考信息 -->