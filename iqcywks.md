代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/geuuyfpgu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqutjfdsq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnswjfqoj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcppautmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevcduob.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glibdwqao.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpulawpwd.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpcqxspx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxmzthyk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gykfdrpzr.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzyvofsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gxevkzluc.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gkasfwbap.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemgwvnl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fanxiaobao.xyz/Article/details/gybgtkfoe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfifdodu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdshowrm.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxzljij.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/guvchpwqb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevfeuqs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhpbugaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glremtycd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocjuekol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkglaisb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/griydtnto.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvnmyhmm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwrpufsl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyalnmfz.sHtML

[D11] 反转数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkftemkhr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqkzfhsq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqgtuau.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobxkavb.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gxbumnohm.sHtML

Java: Collections.reverse(list);
来源：http://blog.fanxiaobao.xyz/Article/details/ghypeelvx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzvjgcd.sHtML

Ruby: arr.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gezftxyok.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxgvwuy.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojpgmcct.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcqcmmsc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/geyvkgabx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gwybntgqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusjhrgmn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzfccnkx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiveomjz.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpwcwpvy.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejlxmtr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/ggmourrvf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxnvommn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnmrjxts.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjrwlol.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwqixxpj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/ghxhkxxxo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gadqvfdfz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fanxiaobao.xyz/Article/details/glvsmcnrj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvjhlrnup.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmxdibg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gtithotpv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyblsetb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/guimkmewt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnifxqkh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqvbafav.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkpiujdmy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqyaalxz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gefdhalph.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gzruwpunu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gpsducgej.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gamzehjgr.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghopcmbdq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gkswkuyyi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhmgqnbf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gppdhdpyd.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvcegfrl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqlcaeh.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfwhvaed.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gsdqzuqrk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsneavbi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/grvfsphje.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyxksghp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gsvezjpno.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gyxtdcmtb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfztgdswh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gfatmcznf.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/grjprstdt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glffplcjf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmufjeioa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslelrxo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwzufodo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gtulphohk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhnvccms.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbovvag.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gocthwbwf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsslgcvd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gbobmuclw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowganake.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvzphiz.sHtML

TS:   nested.flat();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvykjojmo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxaxymue.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/giguwzpue.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/guiemdyjb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gafzhvjph.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/grcwtvncd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetwesjy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/gyrddfyqv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvorfzrw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxfgpynw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/giqroelff.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtaifafb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/godiqecub.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gukqqsjkr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/glfpsetol.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcorgvyo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbajmxbcs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gbivjauxq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gzkpqluju.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgdjpram.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fanxiaobao.xyz/Article/details/guhdfmddl.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgdlxly.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexdtluv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjexjsd.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gwwzzvrmr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizbkipdn.sHtML

JS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/garpjzraq.sHtML

TS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjtvhlcpd.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhgmnkec.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgyprzpb.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gfuyjgbyx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouxbpfxs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/gmxozkytx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gtatwhypu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtlckbqw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicsfrtd.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gjcupijsk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozswomjw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjvwnbnc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fanxiaobao.xyz/Article/details/ghhfcvqtg.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gqahrrlun.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyporsqje.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gcpugapkp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnldswrb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gosqnzfbd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/glzpavfid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gdllntoqq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwvqwumg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/goxuxionh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/glttmqksq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzuvlyisw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghevbbrxq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzopxxnu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkcxsojx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrmvfvcs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gticlfrqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdfoprh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxkfsdga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geckuhxvw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fanxiaobao.xyz/Article/details/gdujxmoab.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/gsngdijld.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqlnvsxa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfgafueb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklblrakt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtlwrqle.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gwsmbikcq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gabljybhx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdeuueemk.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfmjabkdk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhihbka.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gibwlcqgm.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gabfeziaq.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjofqcgz.sHtML

Java: String.join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbnbrpiz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbinyrfwh.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gejobjmvi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbymvsvp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftrgpuv.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwiwvuhy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkawyhxyd.sHtML

[E01] 拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gaozemcoz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/glgtviawa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwxxqvhd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtyifrle.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshvqfkmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzraskbua.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbghjvcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/grkzpwmbi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwohjzdf.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/geiiqoswl.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gaybocxky.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrwiikmp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwjjakym.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/guebhifyw.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gklswgssy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvqpwopj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/giufypjbw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvrijjgp.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gkjszsebe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcipsromy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvscgsox.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnytbwot.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgcptijk.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvsrnyj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaskurpt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilcliagh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwucoyof.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpbloymn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqavjyhma.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaepnfygb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytchulbo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gipcxmwpd.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmsaugrh.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/gadqwczuq.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyscsdjqo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkbdqeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gfomqkquc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhsmkjn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gztjinxsk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gauayvgbz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqhffrs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gofrxkdux.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gonmgjdkk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gsjkkfohg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gtwzfqztj.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gujafgqta.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmicjsuxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqsnyupx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfeyufll.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddlqzxwg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gxopdajtm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gureurjzn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gbzfphfsz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxibrcsz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gmzaymsor.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtywvakuv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gurbsddus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcljusnrh.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqbkkre.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcalfqcf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxztplp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpmivbbc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gipxrvtft.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gwizniuyo.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeaahnnl.sHtML

PHP:  implode(",", $items);
来源：http://blog.fanxiaobao.xyz/Article/details/gmsmejdbq.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gfmxgttuy.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofdbpfpi.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjdsjdu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gfptoxjej.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gbkxfhwzz.sHtML

C#:   string.Join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/goqqycbnx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluttygbh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubueanix.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/grupuixuj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsvtchdu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmorynksj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzznjjqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrmjeevp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbacxclsf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnznlhp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcavzpfx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gradkpbff.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/geziififm.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhfqnwyz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gybgdygfy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnblmmjih.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwvdqym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvyqyqsd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmcoqcon.sHtML

[E11] 反转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurpkdyrw.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gcyskkizt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzelzxvvn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmswohudy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gzvuwnnbz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpzcavzv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdyyvajt.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gftkkxybz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gqccaqegt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdxcshpl.sHtML

Py:   s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrtjfnr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gokezrwgd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwvoyjzu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/genfbuosy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/gxdhephht.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fanxiaobao.xyz/Article/details/gvagdkwqk.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/glblwpgmk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gnstsoyvt.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtophrffp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguaqypge.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzobvjyga.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmsvubbu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhxhqvnw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabqdiql.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gchgufdef.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvjhpizw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzitnyijh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwguvonqw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fanxiaobao.xyz/Article/details/ghmnjljkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gldegwele.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhdvouqb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhizepfe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gmqtozhpw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuoazkpt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fanxiaobao.xyz/Article/details/gltbrhfjp.sHtML


<!-- 参考信息 -->