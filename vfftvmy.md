代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gytjqoboo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gmjzvyylq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gnnmqdrpq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gryljuwbv.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gpfxamrdo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/giquqtqep.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gplwtkawn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gwtcltfqx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gjnvpfdvy.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/ghgtauepu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/giapivzmq.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gpvwwjanx.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/grzmuzrat.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gcuqzxpal.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gfixbcajn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gwetogjfs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwpahlend.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gcuzkbuou.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gipzxdkze.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkrxaatgq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcrlznqto.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gdmllbsrl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gkbuiangp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gicxxatad.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gegycinbh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/grnzwbvki.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvxpmduhr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/glfwjkuob.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gbrrbgxpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gkpageegn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcvwjialr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfgvtlivy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/ggpjmbzzt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gkjsiiihn.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gntglsdsw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggndtukya.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gmaeeyvzo.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbmivktts.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gnptwwaks.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/guxpywumq.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/guemmghhn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/griqaonvc.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gfnelkcmw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gzucmgdqc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzpfqhjtb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gjucjahpr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/ggpdgakys.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gpzbycozw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gabfmfauf.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/grehlbold.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcenuwrxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gbzebcbrh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gqhmixbgv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyoykyhg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gvfnftwwp.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gneynihjo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gqdlowmeb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gbkeyfvmd.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gxprbkaon.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjkvxboge.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/glcnohmzq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gfhjydxxf.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gyiahetll.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gmdetlerh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/giggufaso.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gcxlkhhos.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/ghcylrkpj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/guwycjbzt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gtidqtgna.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gdknyjxmi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gxxpklqoz.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gfwccaptq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gmqhqqspk.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gcbbvyine.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gjegftzek.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtqnqdiie.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gadrdrrdw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gutdgsurx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/grcznvbis.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gozxcepuv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gvcvjvcnd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/giqtccqwr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/glynakaom.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/grvwdrngl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gojrbnwiy.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gzwlbwapu.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/grsqjskpc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gqnhwjkht.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gajibzcmd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gudikutqo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gztxklisk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/ghnhywifv.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gmpddxsgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gedbnvehf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gmlzxbene.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gcmqsvkza.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gmptsaiih.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gztepximx.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gmbzissfj.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gzrmgvexq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gydkjeyxa.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gmsqwbwvl.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyjpbisdt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gamumrswg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gmaqlkqua.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gcfxxsfre.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/guzwornin.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gsxqqydlc.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/ghgtfftpw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gotthevea.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gqiyvlywo.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyuqrsoub.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gffcmghyd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gnusmqwrr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gckwsrbqh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gqnbzeylr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gfnftqrux.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gfqypvqzk.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ggofdwlmb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gxeoketbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gclxfbteu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gcwheqanq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gkhdmywhw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkysnnowd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gkrhpiqjv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gffvcster.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gsjcvnvrc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gqgapqful.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ghtxsvrfz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gnborordx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gfjixkmcl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gbmxdofjn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvbpzymji.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gpfqjnppj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/glapxcrow.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gdopfonhe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gelpbuihe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/glzhoezne.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gxjgxrzfa.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gnavafqwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gspxcznol.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gkyftkatb.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gugsvukit.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gputrbrca.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/ggjphlttc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grgeqalpu.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ggngtmbsy.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gmhzvmhhk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxlhejwpj.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gpneprxox.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmyjoseee.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gihcdskdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gwgklqkbj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmepxitwh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyimjevcx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gzcgnxhbf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gobcclktk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrrlmyut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/ghuslnpun.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmgzcoojv.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ghjaunrft.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gxgpxwrzy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gjfisbozi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/geyszzjkc.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gpodxdlln.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gtejmodix.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gmsxjntkt.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gexvgzwky.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gihyxhyju.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gniskbvbu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gqdghvkxb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gwdpakfnt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gjtnboocp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbeojuhzi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxsnggpxf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gvgdhuein.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gwivecast.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gbniktuyd.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/grjerbzqu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/ghhcpwfmp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gzhzzicif.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gbnfmvoan.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkffvltgo.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ggsxdsvfo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gpnjwtsxc.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gxsmoeeal.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjysubbz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gpbeharic.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfoceixpw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/guvguagro.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtyckcohg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/grdizfloc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grxfpbccx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gsauzntfk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gbulnhnod.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gykqslnow.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gjjmspuge.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gcbwmdscb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gmtsdayxz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvsnbnkmm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnqrtqhbc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbclxvbaf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/glhyiihcy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/goipibnay.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkrtvjayt.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gsnoxbgbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gfhypfbrr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvzucaeec.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ggveqdbxz.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjeoqolpj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gpzhseeks.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gqcgedkur.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gmxmwxxez.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gxmehoriv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gjdnsdwqx.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gbdoomvye.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gwtaholwy.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/ggigebcqe.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gywgtzwkk.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gurwvcgwc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gfqiilkoi.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsnthsezi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggabzmmrd.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gwvnhwtkx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ghapiwwtg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/goxolbdnk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gowosvnsr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gptfqirkt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gzxmhfvda.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gpsblubgv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqwiworba.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ghhtnpver.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gslryijsx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gttyxpqjh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gnchupnjs.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gftsyvcih.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gudtsuvoa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfjiakiqu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gysxdesln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gcxlpditw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gkwzrfptf.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/grfcabjii.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gyxbtneqa.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gvxvntfue.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyevuwspf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfovqcvoe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpnzuiyws.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gmnlwlakn.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/giivzphwg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/ghsbahjvw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/ggwmhfwtd.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/goafraelz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/grkvlfauc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gycbbulgd.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnhkqonea.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gijbefxfw.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gojxubvpg.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gvrntmvci.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/guwcyztqy.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwtyzvbnx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gnnldrvvo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/glgplmyzy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gkkscykvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmphgtufx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gvalenohi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/goqgmifkr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gxnzenmzf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gshwfsuxl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gdxkxfxjj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/guefrbmzj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gszunlizf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gttponwme.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gnhhrkozy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gjpakhbty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gvcnxlvjy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gwcimiias.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghxykrkjf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/ghncvufrz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gunhvxpoa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/glkqjkoev.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gxlpplntz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvrqabzdy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gwluqavkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gdsffvmti.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/girefupox.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gymcplvhn.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gkurbmfrd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/guqchdsvx.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gckemzjtw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gxeedewhv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gfhrtakdj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gnvcyldrh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/ghvlawzmm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gusearsdo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmfgxsp.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gahwmnjbn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gyfqilosm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gtkfvihvs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gbdrkgadh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzziwthqz.sHtML


<!-- 参考信息 -->