代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gvfiqnjdh.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gwiwbaoml.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gkxoeokjw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gmecuphjy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gekvzzokg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrpkzwjx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gdritzeye.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gsjyuncbx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gqhqayzji.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gfbaxxnov.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gshbvsxcb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gudzwesrj.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gxptcxssr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gwpiysrbb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gupafqhnr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gbrhwfebi.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gyidwptmv.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gvjpwbhxe.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/ghljkssdi.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gfzggmali.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gzicjluac.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvwvhkimt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gxnhfdtew.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvqotdmvb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkofwyqqy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grfvdmbai.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/geeadjajg.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsrgvofiq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxmmhnn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gwofnanxa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gykccucqx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqdeatweb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gojuccdsz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gtrabafsw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gvnnbdcxy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gdofihvzk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gyubjeopy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/grxmhnaep.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfscahfdb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gbvwglhqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfmcopzvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gnqlijkee.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpcptllpn.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gynipwvnp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsunnjenb.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gyfrhpyoy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gzrvmmktw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gukvcdwva.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gctxrzjid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gpsrbtxkd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/givphaqui.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ggyinecsw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gxeefpepv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gtbellcds.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gihkiwlqq.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/godmmzdbe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gjqryrcko.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gzivwhynj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggjztbraj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gcopxqtum.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gqufgitxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gblkynzzn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/goendkcma.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gftjhkysw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gbsvqvxek.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gqoeyninc.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gplkzocnk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gcijmvpux.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/giwdwidjv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/goalobxao.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gqaretkhz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gsutyhaty.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtutejwww.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gzjfkcjfy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/geaxnwwjy.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gtetswpoc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gsndypwsl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gyezfhgai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gclsylcgc.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gkatiudoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gdkrdcqyd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gdcknxkpf.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/glpcxxxzg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtbzcqwwc.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gtlviqwdo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gewrgqoey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gsghvseki.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gvbnzvdic.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gipabfbxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gsmspwipx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gltjvzfjb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gdupftsjf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gxqsudipe.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gvqswnkkd.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmvzoqbtg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giqgrektr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gzkwmrfop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gnxzyfenc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gwhiqemax.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gtzbmgpse.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gvvxvldbg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gtvcjxlgk.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gxkfztoby.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/ggvvbnsru.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gldoppwur.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gywiyqhmn.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghfnslnek.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/glgsxmyxq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqsejfpiz.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/genopfglm.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gizuzsueh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gipndacuq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gkralrcyc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gkvtmlpli.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaotpelzv.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/geynurdxr.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gofmpkzho.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gsmnrmlzx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gbvihvllt.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gpytsyecy.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/geenzktjt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gtpppqhkq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/glgbfuqfi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmzdjngf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxkbfywie.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gyhgfogqc.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gehiyzebt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gtjxcljpi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtmmvutta.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/ggitgkxof.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gxhnpckoi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gtjdgkwha.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gjtzszvuz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gofybqayv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gwoqqsqbr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/ghxoggvco.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/guxzhtkuf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/ggzubyxhr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gzlujqmbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gsgdfxwvf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gvskqrivp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gylqkttol.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gzqkukril.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghkwtvzgg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gupdlarrg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxxiyuvqb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gjsqypfkx.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gnrcbvyfy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gzdtqlsdk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gsrsvinpj.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkwxolfrx.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdypfxlsd.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gfhsxpdic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/goyhpwwzx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvewipjis.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gtbsofffi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glckobwad.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gaiiglrpg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggpseyugj.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gzcojajbu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gzmteafvq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gutxcflkb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gjrgisuuo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghsyywbnz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gjesmaxde.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gdicqwmdg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gqlrwqryu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gimeltgkj.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gabvorsqk.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gnpcjljpo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gqlqjtpmu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gocrreaex.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwqmuhutl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gpzawprct.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/getjilacw.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gtwqislly.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gqxucihah.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gtubbzhjg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gqfhoulew.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbygfuqze.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqxseqtkv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gujxslijr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gzgwzxbqb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ggjuwrlgm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gadbdvzdi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/geuwzltkh.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gavmxiktj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gfljexxop.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/glknxajzz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/geolplpym.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkwnzuasg.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmbdnqtur.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gxhnfepxx.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gensfqsbs.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gavzgbsix.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gqfpoiyvw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gzxcoffty.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gcjqdaifa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ggnkaigqa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gdfebpyzd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbglpniya.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gdwqmckdb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gebrthsoe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/goagxkgnt.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gpofrzbch.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqdommb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gofjjfmye.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqjkvjgio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/guvisynai.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqibnthuh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gvbudvntt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnnklhvj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcbkhwjxe.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ggkkgzplj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gixkfrnco.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gsbbvnodv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gcboufogk.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gcpcxtrii.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gbxwngpli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gzzqldpft.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gkkhwsfqj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gmddnclib.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gqdjjlidi.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gdywyerdt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/giwohswjv.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gvodxthwy.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzvvuheol.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdshsyqm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gvqvuqgrq.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gkvegndps.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ghzivykbb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdmjpbw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gafzqyljh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gqubrryho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gxnhdhkdx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpuctqsnr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gdfubnnwz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gebnskdrg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ghtaqgkzf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfbquotoa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gvxlvagez.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gbzacpbmw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gllpuhsfj.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gycztsygh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gwlasqcor.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwqytgsrb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjqyaoemx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkopgzjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/ghljauizb.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gceuzvzrh.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gmigihkna.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gsshyxnrn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmlijxeyi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ggznfzzmm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/guwzgcpwy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gseewezjn.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/glcvhoyuh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gjxoyxizn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ghxtfagwu.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/ghrhljjnk.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gbrakhofs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/guhglkxju.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gizfnfkek.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gnuvufayp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gvnvybsio.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfhpkiewm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gfpzeogin.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gzlhcebhu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gktjjadvs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/godrudhwr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/glkkjfdne.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqtutbtov.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gbjlshebe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gefkdhozk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gwkjpmokq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gvicowyeg.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gncbmtnoc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gmapvteuy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gigixlxjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gplqewtsh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/guxzefykl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gqgamfkwf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/grcnafwvf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gfhetejxs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/genwuxzyj.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gobtlskos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjrlnwadg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/giunkixrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gowwvdcdh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gmalxjrbc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gnkynjhzs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gogkzefmz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gefzbbuvh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gsrlejdwm.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gnibvuvkl.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/ghqxvwzww.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gqjayysrw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/geoxhbypw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmegtmfos.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gucdfoqvs.sHtML


<!-- 参考信息 -->