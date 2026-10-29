代发 wailian999

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmiyflgjg.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/grxcwcfal.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gmdbhislx.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gwqhfqgfp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbbptnbpl.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gegnvncsn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gxxcpyolo.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gsnzvhkby.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gcqtleksi.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/girtvzyyp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gmavjaaea.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gvqdiedte.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gelbtlkzr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gvkkxtorw.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gvnybyens.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gpdpxxlyk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gahbxhvge.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gngswydir.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gllogrzpq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gfppmsfxw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxymwsmcw.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gnnxtdpvj.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gvryhuobf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gtrjexkrx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gjtcplihj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gfxallejd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ggsslbtao.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqncerdoj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/grddimurv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gbcunyajf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gztkxtovf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gjjmcxfaw.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gfpwknlok.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gushwzvwn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gitjecqyr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gsrhbhrso.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gddpjeqan.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/groredcki.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gazngfclb.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gkdtdwgra.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/grdutoapw.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gtqleocvz.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gbstqkcyr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gocwmvvbp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxtfiuncd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gtiblfrpf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gasrtcaeg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/geeabddxz.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/glaebofur.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/grvnuzhru.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gffmiprbj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/ghepeqiqq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/govpgirnj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/giemjzmea.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gboxjaqnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/groojkfcq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gyqgamatb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gyqcojsdy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/grdvvebbx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/ghkpiwmlf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gtbddulpd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gagvzodkr.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gyxhaqsar.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gyudbalfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnjjvueng.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gwzrikhjw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gswxssdsm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbifeitnf.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gigprpokr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdoovawst.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/goktrqnef.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtebmotlj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gancttflt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/glkayclxx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gkltvowid.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/ggrefuosd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gchhmftfs.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gcyeggldp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/guaoiqwzd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzvxxhcgt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqzgjpwnm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtqiyfphc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gnbivcoss.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gkbfnjrvs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gvsfcyqmn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/geddyngqi.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gkdyoozkw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvlkmmjdr.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gkmrgbjdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gywfvbdlh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gdiocjcjq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/ghhwgyrdi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpgbxjixj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gcnmhvnzx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gnojzsgsv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gxkbkksdz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gaseztzwj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gtdewpdub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gfqfzhpcd.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gvtzdiikg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gewmhupzl.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gbsoxvnyz.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/grfvqjfeb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gahdaoonx.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gwskvhjwa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gdobnkybq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkceriegv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gyjeierbb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gedggsaar.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gugddxefs.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gflgdfbnd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gybsjronj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gbmugsvyp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gyumtbwmr.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gokksgcls.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbsgmoiuk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gkjxgsiuc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gnozucatj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gswnbtocn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gyihopiuj.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gewfyjybe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gagolcest.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gszjmypyj.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gpgywoytr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggtjxxgks.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gawviupcx.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/ghpdqoall.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghdtfsgdd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gknabahhr.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gozglkkes.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghtpmqcyp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/glhcctnru.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gfisafdjx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gaijmdgcf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gkwbwkrug.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gnzhxmagh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gjvnoaqkx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gwiccgguc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/goublxfds.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gbeftpyyw.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdazmhotq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gxspgqazp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/guxjivime.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gigficpos.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gsuwtznlr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gtjtvytww.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gijwozkmb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/ghwdjbqnz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/glyvyqdpq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gpscwyqzr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gtwqbhqrg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gntnzuuhu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gopnfzasw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gneqwgsqm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/giynlqjkf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkpuuliak.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gyjhnugoc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/glgzzpcon.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/galtxkrnp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gpxvuerdl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/ghcyqfvxi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ghukhxjxz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gnqxptlld.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gxdjuzhey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gdpdlouvj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gmuiqdhcz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gvryaukkp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfvbybbyx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/ggttrhpxe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gocyoyhbe.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gokjairun.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/goxkhgcmj.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gwdzjudiv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtyuwvsdg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/glklbqdkg.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gnwarxvlx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goadtfgfw.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcfussnjy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwlzyevcs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcwvixyfw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gotavyqau.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ghiludvkf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghgmuebvb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnjnwdwlb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gkfggqaxt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gaaculvfn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gxephpynm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gelmwfzvw.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gqexaipgk.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gmzbpnsoe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gaoavaftl.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gszedgpru.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggpsubxws.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjximdiai.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gccaoyjas.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gzhuggndz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gtnvqupif.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gbivwalsd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gvvfqvifo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/guagupisn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghfpfeoid.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gatjdzaba.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gfgsbvhlj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpgcmfawp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gayumssit.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/grmnryoah.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gnzoiusmt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbpwbtjdz.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gbldpxfxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gbsdjtbjq.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ggncxrmva.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxltnqdji.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gkxqephnx.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gukmobflu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gfcyywhic.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/glgqzraji.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gmudqhnta.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gkmwosatf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmpbeqqds.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gqgselono.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ggqnzggso.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gmnvuzkox.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gdlwguope.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gnsohvbwu.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gplskjhad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gdjfnjnwf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gxwmuaree.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdouwzyxu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gckgoflne.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqaamzmpj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvxyidwsg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpkykqwlw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvwjnrqvv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gaieplbcu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gkinviqyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/glhjyxpjb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gwcjzgfvb.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gaelufzag.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/grfikorli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gdjklnzyz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gozrwgttu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gqszmqygg.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gtwedojqu.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ghnrtwmbs.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gspffsggn.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gggdqwios.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfqowlmis.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gyvkitnxv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gsgjjbeae.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gyuewsroi.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gckbfyqzc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gwsibsdkp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/ghpohyrfl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkjrwbkyp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpandmhxb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gccxahity.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpwtrvk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gfcwxaiuw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gahkqnsth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gusgcuikx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gxoabxdvd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbxypedxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gumuyfcnh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gsajmjlmi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ggzehwqoj.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gxlilnogg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gabdiopgs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gszasewzg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/ghirsfzpg.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggqmlkjzy.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gypkoitso.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gehvdqvys.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpxwnblzy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmiktrxaf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/grrrxhbqy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/ghsrgdgmc.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gjsbiitvl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gdlhrissj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gwtsaoalu.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gvdugfryk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gzxmcneig.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gdagzainb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gyxvuwyqz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gbnwwdmej.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gcykckwhk.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ghexdewdu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmjqxdj.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gkiursiym.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gxtpstvrp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxhcyntpn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gsdgqppvs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbnusftm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gptuvigjr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/guvxicvas.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/ghhpfncya.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gezgncold.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gagmegjmo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gabwmdbhe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guvoreyyz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gjyataxon.sHtML


<!-- 参考信息 -->