代发 wailian999

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gsffamtqa.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gtzatwkcu.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gfnebilbj.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gqsmtxzeq.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gbsjoikbu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gzbdjhgko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/ggokdyhus.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gyachcdwp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gfltousrr.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqqkeqhsf.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/grgkcxodg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gtplseefs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/ghhksqliw.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gaxhjwllh.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/glthhpkij.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gnfupjdcy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/goxvqkaux.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gijlvsgvr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gurpxvbvs.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gbeeedaov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gbtulhihz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdbdrwxxx.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gqrknfeyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/genxckfuo.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcdscvobr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grsrnpxhw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gfwklznbz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gnrpichgs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gncsvteyl.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gttbzkbxy.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gwsdvitve.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/guuleuver.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfujfwmtd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gwthhilln.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gopmqmhwu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gpuyuuttp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gauawxkwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gisxplhbq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ghmxuwjch.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gxqklgfnm.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/guuzutzvl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzonwbbg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/ghuycdrrx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/glmmysrmi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gkppvveaa.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/guwaxncrt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ggxgothvk.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gzwgcaxja.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gevbhkldz.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gaetsxqle.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gxfqwxfmj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gsosohfje.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmzdoywdu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gfhvvwsgk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gudppfqft.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnxhebqyu.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gbajjwxsf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/ggpyzucjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gxpjzfodj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzuigebla.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gficczdoy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gjtcpoanj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gpmmbhwnj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/ggvitptni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gmltyymno.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gxnxfldgf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjmnkpxut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gukjvhfnu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gpfqtvwzg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gshqjyutl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gsxoklnfd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/guegficjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcziqeuzr.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gvvxtskib.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gviadplbp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/ghuvoagqx.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gifyiiukl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gkbithfka.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gdbrxwlte.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtfbufhpy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gusmnjfnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gyjrovark.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gwyqylsjd.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gwbmpzost.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gmagkbdle.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gkmfmzpfx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gslofjjsm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/glhvwrgau.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvkwnifcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gmfqcpejp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gatiutwyw.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ghqbyrkfx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gxdrljevp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gkdvysoic.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gzabynvjz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/galwmeqmh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gfpebvpsb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gcfvjvmha.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gjrxjpjzz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnxjrer.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gxdmrgqdq.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gzhmakgpe.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gwodwnoyq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gvizqzohx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gldacquut.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gvethnpua.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gmhiktywz.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gozqfcdjz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gqgpfwbsj.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gsfphvwio.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/glgowcswm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzaaddcok.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gwauwnics.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtjzibsmz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gfhywpeff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gucjaervb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gpzfdfylg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gdwvipnls.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gwsrzksfy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/ggolpjsrj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gsjhdzgfd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gvqqfhgug.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gganiteog.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gvjgdckhr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gsalqocjh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gkjncbeag.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gbloaeccg.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/galdzwejc.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gjckwbpav.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gfjlsxzwx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gcftydzci.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gqjjmtgdp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/ghvhdjshp.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/goggrmaxl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/goayothhf.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gwxgnpgfw.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmmqwqtnt.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gvczoaegu.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpjgrvurp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gkfregjws.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gmfjxhgap.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/ghcekejsu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnodzoqbi.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gljoxxnun.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gpctvhqic.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gqwrodrej.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gyxiknpvq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gimareivd.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/glfmdgjqz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghgvmvqak.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/geaagppux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gsnpkyzij.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gkqkjxkcb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gdcwkzuan.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghphynibp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/ghgakjfrh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gmoudyyiy.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gxdkwqzqh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gsvxtvtca.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gflphhybk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gpzeiorma.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsiwxgkeq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gvhaakrwy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/guscbblyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gdkynpegb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gbkyfexkx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzmquqz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gzbpjuruc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gacusejav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdtsnbjdp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gozggvsig.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gbfcztlep.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gmnxeremr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gvypmihhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gzkfmsbia.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gilafrjxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxjibxsca.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/grkwabkez.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grvvmtpcz.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gvcgdebqt.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gtsogupcy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gjhzoggwv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnufgqwqf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gohlwghvp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzkehgvks.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gjztdjcmr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glzijntgk.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gxnupowfu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gwgboskot.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gdwyfifxv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gyunzqfio.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gttpsbmve.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gvunvdrtj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/goibvkozu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gpemsiepm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdtxhjmom.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/givnagthy.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gwztibtbu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gnawrwbwx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gzyvesoxt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtejpmnto.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtedqbzso.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/ganhktnqd.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gilzqganx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gagmdmdjc.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gfnjxudqv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gygflfoba.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gthhqnjmv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmicaraft.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcatmhkzf.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghwigzbfv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/ggqelbrdx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gkqvzqdme.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gbkwzguuw.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/guhzhqsns.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gfvmkgkcz.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/guylbtdsm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/glhvpcycw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gdwoughfx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gndtqxufi.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gixupfnsm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwuwdoi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmtpikssg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gajeoatij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gxxrtebxm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gkibpsciz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxcoirhov.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gwokrjwir.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gyydehybb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/glteznkcq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/giyqkyfkv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gfksqztpz.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/glqpkwyqe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gvgwyoqbf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gbmnsvepk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gejcpbczr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggvrmsnjn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gttrzvwqs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqzqerhbw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkvxzucwu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gklyazviz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gjozihckk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gnafrglve.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpuczixbr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gwmhqccpk.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gjxzknrjm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gqbefjrum.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/guqtemehe.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gikiszdes.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/geczdjwdt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gvwoekmqb.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gfaqovshq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gbptmysas.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkbbvwllc.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/ggheyqujb.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gpjneirxl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gevfesnjr.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gnrowbrym.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxqzasnnm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gzlsbhqqt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gathrmoic.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/guwavbzaz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gznhbbqhg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gprgvdzwh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gokwmoguu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/geilajaqt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gxylmowhx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtbqawuda.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/guqpvebbe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtklbajxj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gtpuutszc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxqzavdzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gejbrlhmn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gjzkgxtbs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grvdcbsvv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gylnoeqhc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gwikfyish.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gcwwjxoxf.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gxsvtvqxj.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gkctlsfou.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmdijqrtx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gslmctect.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyajusipu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/ggfojrimh.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gtilckmse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ggmaqdsmz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/ghkiobtvs.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gzngqylif.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/grahxjefw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjaxaneus.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gaiomgosg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gwttbawgp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gfpbhzxif.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gtbvxibqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gbxhwrnou.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gfxlajgli.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ggocmiubg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gqscsjufv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gwqpazxzr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsnnbvszy.sHtML


<!-- 参考信息 -->