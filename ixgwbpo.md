代发 wailian999

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gygxpbbnf.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gbyqvxsqi.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gajinyetz.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gnwmvnkxv.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gaiabuvqd.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfxvqhdfs.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gcbzwfsup.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/grwpgflco.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gmobxqcvg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gowrwyjjh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfgjtzod.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/goineysew.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gullpqepz.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzeonnkrp.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gmgvruxax.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gasslqdsu.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/glzoqbbft.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gcgklvxit.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gixotkpmf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/guobewylg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gwxlogjmf.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gzgpbhcmt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqtnrsohm.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gpfpdkash.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gverdecol.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdjtdpmjr.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gcdtkepyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxyfynseg.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/ggoyqxxzf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gxgxrldgh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjtnjudhn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gyqslgncn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gcajfcecv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/genevcsjc.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gmbyektlr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gienbuphu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gxbifidji.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/ghlrgnoxg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gnpcrzajo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gliogzukw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gzslqhzyk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gwkunxpjb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gnlqzwlhh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gxytakppq.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/ggnblaffi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gfcxhanuc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/glbubxanl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gpyswxodw.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/ghdldxiim.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gxkuxukze.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/ggyfaqjoo.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/grlcgpzgv.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gcckebwto.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gpcbelgpx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gfxwdvhxz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gsfzqilnf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gngpboidu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gjbucmhka.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ggvtkfpke.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gowuewkyt.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gwszhhjwv.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gpaidzauw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gsjymmuni.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/girsabocy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyiwblaan.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbljtpaqh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/grnwxonpl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gumiolnty.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gaoeisehl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/guwdoewyl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghegkrvnn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gkqhzedzd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfnjywjsx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gcvauiflc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ghgbbhnon.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gkmrtsmfc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gxoejlwzl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gduuzkgri.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghrnaaiph.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdzqwotac.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gwbvbhruj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gvkhggzry.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gzuhswlwn.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ggiwytsho.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghcdtddgt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gsytfspyt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvtwrqb.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/geyiemffx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gvlwmqnwa.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/godhqeivj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggkussien.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/giiufxugf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/goyoowkju.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmtgdyuby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gpcoymecc.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gipykihaj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gvzcwbhvk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gpugfedzz.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gdfmggazv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gvgusrnno.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/grhfbykvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gsiywnoda.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/grpwhwjka.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gmxaxyjlk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gzlzownic.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/ggdoozbjk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gffykqdxo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gyqghwiro.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/glptoooae.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gcmgfoygx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gkgddojoh.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gbtlrvvkn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gmgaqnmvo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gyegvhpar.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gxztkpomm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gjgsiesjr.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gmqldgyfb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/grdukwfrr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/ghwvzdqws.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gjewvxnzl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/grqtirmir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gbbsnbhym.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/ggszkfcha.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gpusigaql.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/goffmocfg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/ggaifssvu.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gwprfjhou.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gbugegdig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gwxxndxxn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/giqyykcds.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gpzjvylpj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gvoufggjh.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/glqsoderx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/ggpfjbhzh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gfznvgplw.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gvtwccabb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gvhwuwggu.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcspmzrad.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gmplnuilb.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/garymlmhs.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gclorzyuo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gifotclym.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggiieuyzr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gfaqndjlt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gagdlslsl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gewitzfad.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gngebnycc.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gbvmfccwd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gdhwxtbwp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gywiezpod.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gxhzdkybd.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gqgfodqvr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gisnbqyyk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/ghbtscizz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gsqggklbj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gcxbsefqd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gffsmtnzz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdjlxkea.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ggrxsjflv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgdhbjp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gailyqfqu.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gejzqjyny.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/guhvnljqg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gzdrraeif.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghqmhdmne.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gitojwulu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gjortklsb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/glcmkvids.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gbidoaxhl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gpkvkyysy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gqjnpnmnn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gkzhsmilz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gcnzjtjkr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/ggsgwmpdb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gdrhwnqtf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwhcdatgd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gpkrrcprv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gljsupufn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbicjhdx.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gfwhsoymy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gpilvornb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gmkapgylz.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gpqazuikq.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grxrlqtyf.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gdfzxjmtd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/getwzpaag.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/godwmsxbs.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gvmxwtzwp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gavqqfkaq.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gmwjjncmu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guwdrmyoo.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxyrqbzso.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/ghstdcqtd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gacutlajp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gbciusbjy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gbkdczxky.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/ghkspoltg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gutbawxll.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gyacahvxr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzikongbd.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gdwsgfbsh.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gswgyvker.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gsaqwkmvj.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gdjqfdkwf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmelxzlzw.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gnifxumbl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gzaehbykt.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gqhlhnjsy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gtbrkbpyc.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gwdgwynzk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gajnquoxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gvtorbdvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/glxasrmhy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gapukqhlu.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gjkqxiuuy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gqhmjlpmx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gwlgxlgup.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gkummwrdf.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ghypgppqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gpwforexy.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gbglkxaai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/ghgmfgbpj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsupprgvc.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/girzmjnjx.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gvqfnixdl.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gabxwytht.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ggamizcnj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gibtruxlj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/goetgsasl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gvxpknpzb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gvcyonvjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gqtkpqrxn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gehfudhfd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gjmaboovi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gdhzcjuna.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghscradvd.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gosebsllk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gratlvyvd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gdpsvafdx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gyfeplfjj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggzasdpzl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gyevbzqwy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gbjksobie.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guwdgkkgy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzcqrnxcv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gkbhsvzym.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/guumzayog.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gnewmqqwb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gjxxhmfnq.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gedwawime.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gjtxecqly.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/glkuouqwd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghtkwnwze.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gpwedolyk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gdgafxcbu.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gtgavdjly.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gmzfwkueg.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ghtcznjkd.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gbzakplrb.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gmjqwdvpy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gnspfikaf.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gyzdjxxcv.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gtbbynfaq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gwkpzshss.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gkqxgpqzp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grdhxzuoy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtfgxqdfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gspyqlmzk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gcrxwhjjv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gfxousrnm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/grmmuswle.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/glcjxnxlk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gcvdbkemz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfgszcctp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gvzteoldl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ggtgnblwg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/ghzdoylcc.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ghhnuqzqn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ggqwrejeu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gvgcxbuib.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gvmklrram.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gniuqkjhx.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gjxmqylap.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gvrkicyfp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghdifunyt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gsezplvxy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjeklpfiu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gvmoewlax.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gptbwcdkb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtduaobch.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gzraxreud.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gutbzbkzw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gzckvlepw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gpagwirpn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ghmzwlzfy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/ghwawdbnn.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gpqkrbnah.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gcopjqcwa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gtnujdgth.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gxyzooffk.sHtML


<!-- 参考信息 -->