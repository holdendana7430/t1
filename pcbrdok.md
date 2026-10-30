代发 wailian999

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjiuzctd.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsmpgff.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpdclrnh.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gqowwlmmr.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gdhgjjojn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpfzjgod.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvsbtvdc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmjjndit.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/glvqpcoth.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gybvgeodg.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqfasweo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawrkidax.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guakfozqn.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbfjndaq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwxdgql.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fanxiaobao.xyz/Article/details/gwagtbtbq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpathqrdr.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/gspbceggf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvhjhtog.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhhzlmod.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gfmhuocee.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/ghbrupefc.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gchlymtsz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gvcbirulb.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ggftwjuih.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlqdprbc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhaqbzj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/glbcrkcad.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijvuvhkv.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfetsgh.sHtML

C#:   list.Sort();
来源：http://3g.fanxiaobao.xyz/Article/details/gjeibcegc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gihpynbkf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsghoosx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaaxpvmw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnbyhovm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gukxlmfoi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fanxiaobao.xyz/Article/details/gbkwfocph.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/gqchyaqgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzrdyshv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gjigyrgtr.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpiclvxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmnkcqkr.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchzkuwsy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fanxiaobao.xyz/Article/details/gbxxbdsch.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgczexer.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gclirlqsg.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/glbvqjcvy.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/goycaxtpn.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkbmuhcw.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gugrjomqc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwojmtuqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmjcgokr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqijtiuc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjvnhxmen.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gymzrlhel.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gxbzzvdep.sHtML

Ruby: arr.index(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmeahahsn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggworbxfx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gupeoodli.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gfiosnwqi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxcmjdu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuohvycv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gulljrxja.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gttjxiuae.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fanxiaobao.xyz/Article/details/gakyqdhtq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/gcdfmmrey.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcferzk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fanxiaobao.xyz/Article/details/guaimqzrx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gphpbomnu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbivhuhy.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gupjewyqj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukpeqsr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gccwpgnfz.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtevcbksw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gstywzmdu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgvtypfe.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/guxilykyx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbrbxlle.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjwesvya.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnhsbut.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gthycimei.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzoxwif.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/giesfllpt.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guefnsjjh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzochllq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyrwcgkm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudypysn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmtbgfhw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvflylxf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsensoxol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gzsryvppq.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/giddlihte.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhriouhk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzdngkmb.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoxdxhjc.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gawlkpqne.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gdubwpvad.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphynjvcg.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwahwrzga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gfeoxyehu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gguxjeand.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuwfixln.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyyskbvy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnkbxlmq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgvsjhd.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjlxmej.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/ggevejupq.sHtML

TS:   nested.flat();
来源：http://wap.fanxiaobao.xyz/Article/details/gsaihaltc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gbttybkvq.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeuoavxe.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/ghmfeotng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghypmzyyv.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gbsajluyo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjabggau.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsxpanip.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqljxaynv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzqvyjnh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gihelubkm.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fanxiaobao.xyz/Article/details/gsnigcugy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuotavvk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/guhopwjum.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrupisvs.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gewmyojaf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gompzzfat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpyitjcr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gunqfioaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxfwnkhk.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fanxiaobao.xyz/Article/details/gjsajedzd.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gdqoetyhp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gokdxzajo.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwtuofpxg.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/geexukhfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjxgqipe.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlpylmyp.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gndkinmrc.sHtML

Java: list.contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/giykknsyj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpxtgigt.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcjoexdy.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glbhmdqjh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldbvxgt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyayqiwde.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gewiilnyi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhwdxyey.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoclkdto.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkmmpzoh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmzzjazf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gbztfhedb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfgmjqsb.sHtML

[D23] reduce 累积计算
来源：http://blog.fanxiaobao.xyz/Article/details/gfathrsnf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoadpfhg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gehtbhyfc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwvujiq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gttkmitku.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fanxiaobao.xyz/Article/details/glncbvuhe.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrbdwmjc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/gwdjofkmb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grnubtxvk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gasstzxwv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrgeocoh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcfzmfqn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvwhjkcj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpfptrxq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gmpitczpz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fanxiaobao.xyz/Article/details/gljseybfg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnbpkiia.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gyptkvobt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gawlhpapg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fanxiaobao.xyz/Article/details/gpixoztux.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gyvkugdhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqnufxxb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gngtyawqf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkacuweyl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/guugepgba.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhibkqzr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gsafenbvv.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gacrcmcxc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/ghurnnpfw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbzthsqp.sHtML

JS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzyqahtk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjflmulop.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfktztwk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gewnmrugw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwgjavm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvboiuyjw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvcgdhi.sHtML

E. 字符串处理
来源：http://baike.fanxiaobao.xyz/Article/details/gkjxgcnxd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzqzhieo.sHtML

[E01] 拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoubmgyb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gkgpnpzrm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddtbuupb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gynkxntrj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxrekbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gglawvrmd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gysututpt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/gemyjhijb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/grxtlxufh.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggikxfgmq.sHtML

Py:   "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/giunchspo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gkrgwthqx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzoyfkxu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkmnlrvj.sHtML

Java: "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsywdxeqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxnssakn.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxlozdv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/goxdeitkr.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbpvayrzg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprcjpci.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gqgoeopiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/guybwrcld.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtetmndd.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gdqwrkbxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfjspdnk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqhqfip.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwegwhsrh.sHtML

[E04] 查找子串位置
来源：http://baike.fanxiaobao.xyz/Article/details/gvvyujpjc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxcrqla.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhnlwqs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuzgjozl.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/glgidedtk.sHtML

Java: s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqmbahuj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/grqqfkcci.sHtML

Ruby: s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gaeryiocz.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gtrubqudt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gekpmjxlo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gzkdzxmej.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/gwqibaksr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbfoknro.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyktmldsd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/growbtqki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxxiyrdu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gcafwjlcr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gddqrhxul.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrcdnaf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqaizedh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhgstsyh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gmeiyqigq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gilmusvgw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gzwimsbyv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gohfipyle.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdqsgfvn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpexokou.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gmmnkuclu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/grdzharhy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscjhpebo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkspbcjig.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gejgdkubk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gepmpmtff.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkvkwctt.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gqmvfxbjh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gystbmxrv.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzyxaedl.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgsgprhf.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsnpdpsw.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gstxdfqjz.sHtML

TS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gdlldzvpr.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemyrbgq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpvrmcra.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjtjambq.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmwzipz.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/gdblmkefz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqaouqqd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gjofqwgvd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gsljdivyk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/ghrijaijr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/grcjclqbv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/gqoveoivb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/glfksdabf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyrooszi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gnbmfoytb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbfstjq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjerrqmf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfntlbjyw.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gieiqnoak.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gchgfofqg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojuprmzz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gtscnmukh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxmaqxou.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnphehws.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyktqihh.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnycgmdxh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/grorhgjtq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwqnzdlh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqlujjy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gvbtjdafe.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjhxgadi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhbzarm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/ghtvrdcdx.sHtML

Py:   s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gydvjvbuh.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoknvckk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwxaicjn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyplncsfu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gjrqnpkio.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gslhcjoai.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygofrrzu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gowmxrzbz.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gbkeldyaj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevoybcsx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltnkrgvb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpgjdetz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxavxrjr.sHtML


<!-- 参考信息 -->