代发 wailian999

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghmqtonpt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gzbiizigu.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gupoxnfxi.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gijqmptzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guxerlhzm.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gogibhimi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gmbdjbxir.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gknzuylqw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gkozhqrbc.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gchahbxff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gctcwezmm.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gpmkzziom.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gadmuthcv.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/grdjvflrk.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/glmyrivwy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gqfubgwge.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvsuwrjjl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gjogtbznp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gxjzmrzwf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/ginegcnns.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/glezwztyz.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gfoiddrzo.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gxehlpxoo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gvwwsomek.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/galgqbuff.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gmfvmlczs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gynxpuumm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ggkknucjq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gsvgahktw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gfnjwqvar.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/ggjezccqh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gnxsabunv.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gkcsvqoit.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/glfzachbh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/govanzqqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gdhwvgicp.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gjuitcopg.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gygeidvwc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gitobzdse.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gprkjgzhx.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gawkinqiy.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gudsofnrn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gflccqrmp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/glfviruzl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gwtlyxrxu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/guvgnebfr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/grujihglt.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqqpcjkzd.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gruajhadt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gizxpxvur.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/ggfsucwnc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gcmosskty.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gyjyffvvz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gzqohnmzy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/guxdsjcmn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/ghuvmptib.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gjurcbrhe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/guaryqnac.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gysascplx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gfywxtoza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gkgkvagot.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/girsvgkjk.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gxppyatmk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdljconn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gplmnxuvw.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gmyjwrbka.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggtysnerk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnoqtmmoi.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gptfqjjcb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gyvmhojfs.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gdkxjdjzz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtlqcdlnw.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gljgsgsmw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gnhaudvye.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gtywysnji.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/grjnyklrs.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gozubmuwi.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gidxwnlpt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gleiisrrp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gkmcabbeh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdujuhhvh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gimnznsnq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gczdzllis.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gkpcprumi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gvfozvukt.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gwpwcrikn.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gruntmixg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gfgdcctcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gcbnstjge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gancsrbue.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gwonnvahw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grraeegyt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/ganngodgu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gozvalvtf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/ggbkolihb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gdfhimeue.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gwngmmhmk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gfpmowcub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gddbdqpof.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gzyxhoxup.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsfxkgvbk.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gstlqyzrs.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gvhuzayys.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grqeaktuw.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gerooxiav.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gohufwxge.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/ghqscnbno.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gimhypjea.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gcwkezxsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gqxeqdikw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gnuwqjwuu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gqhngpjlf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gtutfxcfe.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gpzrkpbhk.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gtyoutvtd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gsnkoakat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gebkuulma.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/guwxsjgnw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gdsqvdioq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/ghyoxhbwu.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gvvwyqtay.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/ghdeawvrb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gzbosudwj.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gnumvwwfg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gdbxmwxns.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghrqmthlr.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gagnzxday.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqvpxbvei.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gstorkvhf.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gikkmmhrp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqduyjqal.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gglresqfp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gtioqikel.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/guiwglesd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtdtaywkt.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnnyxwmdq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqkiammgb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gbvqwdhed.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gwlrzayum.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gquowqlvm.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gsbowgtpo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gpbjgfyxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnzmqqzrz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtnbnwmfz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gamruvujt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gsgtlfoyk.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gbzuqgclp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gzihcodgh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gsvpcdpze.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gaybzqvdv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gvilxnlap.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gyuzvhjeb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxguohgmb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpwnxucmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gcgbezrkn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/ggplpptvd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gygojpdtj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gtnapuvub.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gmvtsthke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gcuwqzjgn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gndnrbwtk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gyuixcyix.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gnvacesmk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gagwjhyuc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gtswwwvni.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gbrwrmzlg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gloypbqjq.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gunvpdphv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gtzdujivl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/grlhigvys.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gbvplsgdm.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggmyrsbej.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ghcmszljl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gkyemyjkj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gglbkrdiw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gusfxmvzy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibjpurbp.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gsdkxsihw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnehspxql.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/guqcceuny.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gzntavgkf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggwrbdniu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gafzympzu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gwsydpawl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gkhbztwlr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gumxudvev.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/ggqrbumiw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsptjqwyl.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gisqhvcct.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gplvsiasi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gqoyulzsx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gotoybeca.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gwgpobdna.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ghclaunun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gwqlqywru.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gymrhkqom.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gokkwgdkl.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gukeymgpz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gbyhhqjhs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/giurnaclw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggokegzdg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gyhwsuldk.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glwkysbpc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gkntqvuni.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gqetbjzyq.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gpqxjjbqd.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gshtbvyvs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/grwawksmg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gcajmbekp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gfjbxlnsx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ggctsrpel.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpwumerqf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gnulxvjrb.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdggvsyuf.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gijjezsmo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gfpfsjjyl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/glmotvwjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gwxqznlvv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxxokkgko.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gwlueroyy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gzjsdfcza.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtqaqkyq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gwilqgroy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gtdjkrqrx.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gehgsyfba.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpswazuzt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grxnxgtrj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gspkxwihl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbawlewal.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gngetnjtw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gaikjnrcq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjdbxuphs.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gevdzviqi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gwoxfafjx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gdwfpioep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnwtggxet.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gigxnxpeq.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpnwybyad.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gpytzcqpj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gsgdbyimt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gptuobeua.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gdhjkzuci.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gyewjzyow.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/grdrrjemg.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/goszuzxim.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdguwjvl.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ggpjvwavy.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gekfxtrmz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gaznafltt.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/ghjhjhgcy.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ggbnuwagl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gwdtunslv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gqgpmhjqq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gqkjgcxch.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gephemqcw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gggctfkog.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gwvgqqoqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gsymhmftm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/glcelwdov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gjadydjvi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/giknooeie.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gxkkptari.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gasmbrixw.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gwcyuwwbr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gcpjkomvn.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/goqzcvqsd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/guecvqjer.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggdesvjpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gvahsyxog.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gbjxasacs.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gcytonljn.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gtrlmaeco.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gpzyqrqgz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpchrtqwc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gthujacwb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/guypclwkp.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gleqzkbvb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gntqrnetr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gtuviofmo.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gfqfvbhin.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gzubfenwv.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gwveeqttf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/glgivcjhs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gupvdhiub.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gplbrjmlw.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfaugwcdo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gfbcdxzlw.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/glmjfdwxb.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gehebbofj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaixdupwt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gnmilebpq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gcvsklwyh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gciqzmzne.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gsfzltlqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gsuwikmsx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gngvyobfr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gotkspbeq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gubmesxcn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gcayihgem.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gzksdewie.sHtML


<!-- 参考信息 -->