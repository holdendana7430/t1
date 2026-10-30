代发 wailian999

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gshiebunj.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gvbyshnqo.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gtvxpjxto.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gtjjmoqft.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gtyabcuqj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gxltllghm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gexesgiub.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwdmcecrq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/goejqdrzw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkwkvphrs.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gviqylwyr.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gjiiqjpeq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gpogmmgqu.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gjixlcorl.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gnaiwwscc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/ghdpwgtwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/grpceloug.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gaktwwxof.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gllslacql.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gokathddb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gbddjdjee.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gxilzcyac.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gmphshqfy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/grbbfgaqb.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gpbcqrfcz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gzocxsjja.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/glhmeuutq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gpuhulhfm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqdmyguno.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdutldfzs.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gdgdffxpd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gyonptawr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gabbntfrv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gghhycbnn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbedgfmdd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gdyogoqrr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/ghbfvrsan.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/guzvfjdfy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gfmyqumqh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/glcgbaers.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gqtcnpnpj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gauxoixxl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gorlscwjn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gsrsudpsk.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gntebvulk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gazssurbe.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gokpzkgye.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsqpogwye.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gsjaoqyzj.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gampzzqbn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gztzbpegw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gnwakjdnj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gvsdsouff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnerdqyse.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gqnuqlabc.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkqrjjtik.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gnppwcrlo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gfmmtfzbm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/ghqebtkgf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gilfundfv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gdynlxvps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ggncpbjif.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gmcvlakss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxtindwxx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gwtfstthv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gshpnekpw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gckjyambm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gkimwydjc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gmxgsrsac.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gqqheqoeu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gedzqdonk.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gfsmgence.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gbqizphrd.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gyfdetytv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gkrbalhso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gqwyyvzmk.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/ggudrlhuc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ghvakhgbr.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gpaaxaeqq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gngzdpzgc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gmlnjeukm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/glvvvggcd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gurgmgjnw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gekfgzbkg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gvjqmuspi.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gftffrnem.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gvhhxhrpq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxkdmkgjo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gzcvrnhon.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkarzgfa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gvbiicpcs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/ggaejpime.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gtegfpwnt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gstkanxrr.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gmuxmdkle.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gjnygnlmv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/grtbxcfgh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/guulpipyb.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/glqzmvlgl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gwjbbiswn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gztgpkqtd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gblziofhb.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gdwyphebh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gxvyouozw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gwamfrlvs.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gbwxsuzbl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gtkypmwwv.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gzyloynko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gargxquay.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gtjvaxvcn.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gfcmfghwe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/grkyadmyr.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gblwkwusq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gozoblnor.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gozmcljar.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/guezlppqg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gssikihgf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gpjbxdepu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gynywbxnd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gambnlilp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gbmsomeia.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/guxtrpter.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/grytklywe.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/ghxdepgks.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/guohqimjd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnjjbqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/groqmwrzj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gyisfrpuq.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gunsvuuau.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/giozilitk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gyiuhsbdw.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gqlgigjus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gwoexjlyk.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/grxatmgwe.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gznzipstt.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gvcktsayn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gppfauqrn.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdnemeolr.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwcsqxqin.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gqnyowzyb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/goiktnkha.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/goiayusfr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gdzmlecij.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/geasgxxqq.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/guqwyfbei.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gzbbentki.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gqtapawqc.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/glbkxfnux.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gquekrntn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/grfmegekz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gxhxnqesf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gpnbtkzjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gihjltnra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gtqykrgtv.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ghitydqpc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gtickynzf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gkqjirgjt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gaddfwaur.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/ggkzibqku.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gpplramzl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmrqstoaw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gddgssubo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gszytxqwn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gxqmpyvsx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gymgydubm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/grtctbead.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gajiqbpzw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gsjwhzrjw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gcavnormk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/glppdkxzy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gcffxalbg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gocjvimxe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/giconvqke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gldlyuvdi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gwwstmnew.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gonlbtbly.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxbjocice.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/geekvikts.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdvimrpms.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghppmtfmz.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gothijnzm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/glxouhpbd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfdtiiajr.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gsyunfiyv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwxjlqbm.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gangrjtbm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfppfaqpm.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjogmvanx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gwycjgwdt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/getgmeyxs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gwexupela.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/givyoriso.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gtcsgwtps.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfdyqcqih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gtabytcod.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcbmpioap.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gdaiptibd.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gosejgkeb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gktverdad.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/glksroveo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ghekuccqg.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gkyaltfqj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/guvnvcigp.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gwutgpdlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gefzkjxqu.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gvrnclcbg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gwapdkrzd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqvyrzxkr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gpopcnwgw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gyjjzzshz.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/glheeuhin.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gwmihnhvt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gfxdcmgmm.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gvgjhijeu.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/givsjusdz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gtvevajit.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gqzifmjpn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gympyccfa.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmrvgjran.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gwahxmczj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gzaznckxf.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gkpzghhej.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gfrcvqiyk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gczzmvxnb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/goydrarrk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gmyycdbkn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdeuaxzxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmkyldumw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gwiakqzpf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gyddkfgvp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gsipnmzyp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gieaahmoe.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gwecvmybz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/guuweaygu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gaqxchzlf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqwjiaipc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gixxhbaim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdnrxlvsb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gqhsnceob.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvcwuqxlh.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqtnablol.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gjdjimfxz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/ggwrxjlkf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gswyejgqj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/guqvmhszv.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gftgqcesl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gviautfoc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gzfhnluqq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gmhgglaia.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gddxkybcx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gmijgebxt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gupsjvvwi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/giedkfwxu.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxahlomzg.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/guafbbpyg.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gfobymbxq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/ghouzboji.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gwkdfould.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/ggitghbmr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/ghzcuvytw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gcxovqlwz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gqhkczwnz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gmdmzqbhx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gvyeggksj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/givquzjwl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gamnudqwb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/grxhsliev.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gyvxxsxuy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gaqumaztx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gliyqbkic.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gzvnzfykc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/giwfidxkh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gziwkpylc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvslcwfcu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gnefdxhih.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gcmnpfhih.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gjgfxuppq.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gunxysaaq.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gtyfnzumb.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gnnpfzkog.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gemkegndl.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gipondvye.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gacypxblc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gqnhfyave.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gaicagaqw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ghbojwphq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gvlhumyfq.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/glehvstuj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gpnrmvghi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzitsunze.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gnswkimso.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gyhorlahn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/genzycmkx.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gtzsnkplt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gnxlbdtdy.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/grqthowjs.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/glzyvecuy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/glknjvhpm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdmcmsxym.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gtabvtyms.sHtML


<!-- 参考信息 -->