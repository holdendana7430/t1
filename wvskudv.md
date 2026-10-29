代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/ghchancxq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gucaesoya.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gxrnennwl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/grleuzymy.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gyllsbuix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gljspwsgd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gzdecernp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/glwjlvfqk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkqoadwgi.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/grmipqjbu.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gybclicdp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gaifghxel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gyukuoucv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqvaqmyda.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gwtlgorqd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gnfdakepa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/ggdcgyajk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gusmczktn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gnljrjnav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/grzbbsqjf.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/graroqrze.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gkyduogbb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gqefqpgdm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gatphpwbd.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gelgsmjte.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gaeylfprm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggerxihhf.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gcpgprhdu.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gmohuzvzq.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/ghonbswut.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/glydjmcpn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gtxresumq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjztwfxgj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gfjbgvylt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gdayudqbe.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbytzdw.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/ggqizgbnd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/govcxrqys.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gtqqitujr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkjrqupdc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gflebwqen.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gfpvytigm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfwqcmgyz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gtwdrulrx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gugugtrhu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gxadlflrt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpwpbgmey.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/ghcbsuqrx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gnvayvfae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gbkuxrluw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/grqqovckt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gpfwzxkmo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/glapcfxvz.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gzbfkgxbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gpxrrvebv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghogxwept.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gpmjuewyt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gyosdtipr.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gljjjxwjl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gdkbpbbrz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gvdfhgtoo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gqswqxtbq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gvzfdrzmk.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gxdmvluib.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyyonpknm.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gsljepclh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gwdftuwnp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gagnsctaf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gshkaefrp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gttgtuaqr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/grgtizjii.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gpuynppfq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvbdltyuy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gznzqowse.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gguwjtcxk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbwrlmg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdzarmeic.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ghiusrduk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/grppeemee.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gmuuyzfow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ggpneknoh.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gapzsahqn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gydbwrwon.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gyycpjcix.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gmnfbotnl.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gqcwohhzm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ghiqvozvd.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gpokfzvby.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gwehqdpmo.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gyztvdnpp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gilqnziyv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gnppjskhp.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gaewvnbvl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gxkyrbbcq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/grfngpnvx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gtnmhbwen.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gutkmzans.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/grwifppwb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gxxnrypdi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gbjnxajqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gpwsralph.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxdlysfly.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaoyaavbf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/ghxnvreyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzqehgbdc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gsdjqnuus.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gqbfadhrv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/grokmqgzi.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gryacnvli.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gzzhqnhft.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gurcydnkl.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/ghyiefumq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gnlyfnbim.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/grmnrqcdn.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/giokheiwl.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghynofvjj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmhvkrwja.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/ganpicfru.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gxokuwuxh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gmgymfkqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gmrxbxsib.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gnchjahbt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/ghhxwqbha.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ggkjixeog.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/glzecawos.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gkjzszzuu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gpowjdrrx.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gfjdeukge.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gdmtmmzvr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gynmbzlmu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gqgrkfchn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmqfsijfw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/guyojqxyv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gkvcniijt.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ggcgaqjby.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gcvcqoabr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gvxoqlthd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gczxsbxjd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gnftuwfmb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gkzxdeexo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gujbcebpi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/grobhovzs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gcfdewwpy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gtymcgrqn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gnidgwnwh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gwoaycjjf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gvdnclfab.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gnuwlglss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ggawkewla.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gullkqugc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gkteedipo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/giftrtfrt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gywpkvadk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gsjcqvrfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gxsgjkyzs.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gnjhomkmd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gduwerese.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gxemtgihr.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/glczjwxjj.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzhzktfay.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/grkybbngc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gvcvjxbig.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gkgmhuifm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gyfliojyh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkmwjnsqt.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gktovaoer.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gagmrvcvo.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gzaeshsod.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjwhgcpvb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gnymmvqne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gboskfhdh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gpvunusbt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gvgvrvwtd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/glzsovoxv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gzmkgwujx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbcmbnizp.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gykdqjcgh.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbkzjvwfa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gjijeinkm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtycedkil.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/guhynlfdx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxoiecqsv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/glizcljnt.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gwjldoqvj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gbnloipwg.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gtrnbzhkn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gmiebzkgh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gawwicvjk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gcqsmdqom.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/glcxktrxa.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggueohnns.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gzlkhntmy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gubyebpje.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gxabndjuh.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gwdfbbuqo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/glxqntsgy.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/grfoqoafg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gxqgypaei.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/guusefvji.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/giojlagpi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gejxqsbdd.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gmzrzqznj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gfosgqzec.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gnzfmguld.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gfyoimxxv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gtfkhdknq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggbdvvkju.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gudhktfbu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzpythadw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gvlitnunv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gqxmvkfbr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gjpzudsxo.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gbiasamrb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gnaitdmvf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gxnwjsjzl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtnyfieog.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gipgxukgu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/giejmewls.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gbawupvmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/givqkluef.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwvyierpl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gqpzslcll.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gorgdjvnv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gbwqtmhsq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gfpjjchhm.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/glfprutaw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gvmnvrshh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzdzggcdn.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gpixopcwq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gnrfklici.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gsjbwqlpb.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgugkkcj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/ghzyxtifl.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ginhognmt.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gnscmbgcz.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gtplwnlgu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gaddkbndc.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqkkzxmhn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmscxljd.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/grnqwlnbe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/glzjxyrnh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxtvzghip.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcnssejog.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gqgoyaxrx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/geydjnvpc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gkclpljpx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjeqmxzqz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gtavvvvzo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gcgpxeuel.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkwyvfhsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gczoybvsm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ghkjscllm.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtjccnrlv.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/guqcqldoo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gsigzwnvv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwhmxxsew.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/goevnkzkv.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvrkjhcql.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gfxpxzwpx.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gdgnxazkn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzkkxbrxs.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/glaxriaka.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gznwhuras.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/ggbaxwkbi.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ggalmvxdq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpmrxumug.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gycrimngq.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gncmpdtli.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gnirxhufx.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gymisjiyq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkeyuqmqg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/grlhhzhym.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gnahsomdx.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gueycjzrh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gsbwkpbzy.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gzxcpqbug.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gagjdxtbh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyskdkxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gtlpktapp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/golkgftwl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmbcnnzmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gcjiugync.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gaijdjabl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/grevpbbqo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/guorgkjjq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gtcxbasqk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gqbuyzdla.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gzunrxieg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gehlgavgh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/ggrlgkhoh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gyywxzmlp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/ggzbfppii.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbmjercxf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gkkwdinod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/guhvrnwfp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gcaktzjzl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gsghtghxc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gopfsrcsp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/grerzvldg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/glpigoitp.sHtML


<!-- 参考信息 -->