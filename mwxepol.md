代发 wailian999

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gwzkxooce.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gpfhavdvc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gjsqukqhb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gnydkaacq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/ghvmcmgak.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gkisayscu.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gdgmeptyn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gzxtpnenx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gefgulheq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtqzwudgx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/grgmccoud.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gotwbiucg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gqcgsqwsv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gqifuocbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ghqbophmk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gyhwimcuy.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gweksxyxi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gpirmzzha.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grekpbekz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gahhqnpxv.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gxrzlqevd.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gjnpoyytd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gjkndqasg.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gskagbpqv.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gagunehou.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gymzqnigw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gciwxsyfa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gbverxewi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/glkpbuahq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gxmakpsfk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gjdeaaooi.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwsnwecck.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/ggmjcrdgb.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gccxqldau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gyibtrobh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gkshdtslp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gobnpcnsm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gncebdtzh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gphnjsxqq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gayjzmwss.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gognxcjow.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gykugnruj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gqqoomrfv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/ganklghny.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gyxerztgq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkdehihva.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gjeplipnp.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnkdvtwcp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gqjkoickv.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gyyjfkeyk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gfrwjsbhc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gzgqkdazd.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gyouxgggl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gvaohfter.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/goovbebth.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcmuquulv.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjivlfbow.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gesgwljyo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gdimcgale.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gayrtbqoq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdtlpvlkt.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gclzpirul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gwzbnkbfy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzybtnzjj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gltanzerx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gequfmsda.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gqmdzhndw.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gxcbofxfj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gcvvqsamu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gzvwqulsa.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gwwfjshwv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gththzfwx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gxgucxckg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/giotgthal.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gtmkwqgqf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gcanipksw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gkokpuuah.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gggisokrt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gvcfzxzby.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gbbvgqbha.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/glohytujl.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gedtugype.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gklhrbdoz.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/geijbkfyn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gtabrpeoe.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/glvavbniq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gapbqyahm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyrmmkuqu.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/ggmmgeavw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gkipvycco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnzdkiv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/glrhnobdo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/ghrmyfivz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gchgptsks.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/giyjrcdkx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gqyaqdnwp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/ghhbnhyor.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gdxuehsvc.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gtujoyrfa.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjwjjolue.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gzrzhhuoy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gkwwvjeqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gakcbffmi.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gdvigrhhk.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gdzldhtrr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gbqtxmocy.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gilcjbbrp.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gubcmmtrf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gcbwbvseo.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/greapgjgs.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gszrpizmq.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gdutjhsxt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbysgeglf.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gfxfhvxur.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gbrggkxxi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/giklptpko.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gopbspfwe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gfyqxtknb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gccmotnvr.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gsudacypp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gzarakgvx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gmhokahzg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gskmweklz.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gzzdopuer.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gftizsxxa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gwudiyxqe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/ggtfkdvbx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gfazzxfty.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gaxkborun.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gafindgox.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gujonyfqi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gywjqlucv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gumqvtsia.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gdqqnnpsf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gxgdgpzin.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gmfwfljcf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/guqyemjep.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gnqmtfbpy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gtbfwftqc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gpmwmoxoy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gauhmuneo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gxcbhwxvr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gapsjwmcm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gexhqiqgh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gleiqtwxx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gqxhogigd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gvyusvzgq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gcpdpappf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ghomoimmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/geqyfcfxu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxgaowzsa.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/geemczkfy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/guknmglwo.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gbeuubhff.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/guputkdtl.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gsovebmmr.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gqcrljqpd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/grbomqygp.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gnukcpocv.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ghqbshbeh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghwwrvwar.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/ggkktukux.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghzzjutao.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtskzqbbw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/guywqzjsg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gzeomqzyc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gibbryydi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ghfbbvjzb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gjorhmvpy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/guvyojiam.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gwwjukbmb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghtefbwuj.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/grgdlfghw.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gfosyghys.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gnqihosgs.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpmyklcy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gsnpubxdw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gegjlimil.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gitdmjzhe.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtgitercb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/ghfebrszi.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzyhwmrxi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gwhunufph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfwodnjbs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gwmxamgsi.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/goyaeqpcm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gjmoiichn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gacfqkjgo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gkttoudjv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gkgjnznkm.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/ghxthnayg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/glhftjjwh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gfbupdjfp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gwflcjupa.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfohdtmon.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gobtehdbn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gaowzfkho.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gzvavgvrt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gitkaofsp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gmwlilbqd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gtunmiiid.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ghdwwcqyi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gcafgdsbz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gmriyxaru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbwiotpmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/guiwojrjd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gzpyltuhe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grdamjbab.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gwioydkgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gijngvqew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/ghglotmck.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gboflddio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/guljsbbhq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjgxcxyjo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gguveopyq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpuordvck.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gsnzwgcrz.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/glmztqhch.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gsjdmtfjc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvyqgqlqh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gecsotzkk.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gdklbwlfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/guaokqqiu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/guwxxgidh.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gpaznxsup.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/grzejotgs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gvsbchnye.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gwtkgmqqn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gbvuywduu.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gepzwcnpq.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gyqwpsnbm.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gcikjjbzo.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gmqghprcr.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzchgxjei.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/griyulusv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlkbnuh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gshhtlhlj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gukyrgsvk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gsitrqzet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gcgtfgwuq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gxoasuddr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/ggprvffai.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gssobnpiq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gndmczxlq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gmeqxuslz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gnbkvsaij.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gnwadiqdp.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gekmsmtqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnszuoxpf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gppyuexip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzyjaotxz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glubkeepo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gtuyfvlrx.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gzpqvhbtl.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gtankuzja.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gbtwwsare.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxscuqqaw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gagfyhhvx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkoqrwsnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gtpqhikon.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gianqewqp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gjzgkwwpv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gdzwbjiat.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ghofuqnwo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gpwyoewyb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/grxeymjgq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gnzhiwxnk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gkeiokhzk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/grrxmzjgv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/guefgsrkr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/ghfuuknkm.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gpvlvdzvj.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gdptfjvnb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gxtvflyux.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwelyqi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghvbtvzgr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdasexzbg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkyjjfmtu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gasrpbuct.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gsmgqxlqd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gsnxotvbn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gxfttqhuv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gnsriydtw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gccyneocm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gistrfaiy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpvbayhll.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gdsceoewm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gwvsfeypz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gfavyulkl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/ghmqtezsr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gbblwqzbl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gcxgpbcmc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcvsjlk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gfajcvahb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gycsfhlux.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/grhwwllmr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gmtvgnhsr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gnbetrofv.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ginhexxoq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gakobwxxh.sHtML


<!-- 参考信息 -->