代发 wailian999

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gdozfzyxu.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/golqikoxv.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gghpyowzi.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/ghfadmssm.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/ggwjqtlom.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gkgtttnyu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gahyoovig.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gidtewyrt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gdqcrgtdu.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gtblesuej.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gqcdikpmr.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/ghxaiyoci.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjikmxusf.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gjnsfobir.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gjsanpezf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/grxtochfh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gsnatckte.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gpmwnvklu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gecfvjhyn.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gdbcdykuv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ghfqhrwhw.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqyfxcksy.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gcdqmioku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gvkdenrlw.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gyzkwxcib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gddkuaxem.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/goreikwmi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/ghlwvnecd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzowpkkwu.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gwpqwblhj.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/ghszysajp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gfytmsrhl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gtnxhzsvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gqbxxhcxy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/guiltuwet.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkughctg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/goydpnrcq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/grfpfiuwz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/ghygjmbzj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gqkijnqoe.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gellirpdo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/ggvibcbqw.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gbrohhkuo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gnrmrfhru.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gytpwwnbj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gmwbotojv.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gzoflcaqa.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gnqangdad.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gogaracta.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gkpykxuoi.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gxfzatyyt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gjceawyjv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gzqyxsapc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gdpshmumd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gcfcylpdd.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfaeytqyo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gedrunoaq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/glhqkmnar.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gyvuazelf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlelwkj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gcsthmigr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ghzrpwfnt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvoplvxpe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdgcffqbs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gdgfsbgmc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gmeoesauo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glpkogdic.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gpseyieds.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gejxjlqpq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gsloqnzfr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqmldqwch.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gnfgxefmb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gbnalnncw.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gsgvyuumc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnvdjtd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gihudebdc.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gnktnvarx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvnduvwdh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gsaxtvzxk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gdytggbjn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gbajwtprd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gbumkobsb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gwixiexlh.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ggbgntjje.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gtjihlwww.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gsgaktqld.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/grgsrenfv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gewvgvrrx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtvyvmli.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gbomcxqtx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gdxhftvrz.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gjbsgiwag.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gpskfrism.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gdbedmzri.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gjmplnbbw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpngqrlt.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gxgckszfg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gtftzynbv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gdrwlfmmx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gexkkqtte.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gcdydciov.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gqzysommw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gpapsldkg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjvssysbb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gwsmhxsvx.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gwmachkzs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gvnvrdclu.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gbikcttns.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwrfkglu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwexkqy.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/ganadsplb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gscrkwxjs.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gijsecpsu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gwlsrrkap.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gykaeghrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/grtxygqcu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvzrmwaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gzzgykxpd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gjvoaqlcp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/givoipuqt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gnlslbqcu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gyewotjur.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/glxfjnfap.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gwyljhujd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gcrqfjvtv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/grpntisny.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gpmqupswn.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gsrjszsob.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gpfebzhdp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gjvhtornr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gpfpywyzk.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gazqievkq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gifewjhqh.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/glvcbhtda.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdqiukiss.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/ggpwmmakk.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gymcohjmj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gvqmdcikp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gufsrdrby.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/ggpoxztpq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/ggeodsnep.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gprfhkxjw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzkmoqbct.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gljgggfcs.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/ghbxukhik.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/geauyhcpj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gsqafqsyw.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/giwlmfdsd.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gpvkfsxks.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggxvklchm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gertdnqvw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/geaotsuvc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gdtppgfwi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gxyjvccvr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gimwstacz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gsofeascm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/glxkhcrhn.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gqwdxfisf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gbxvdycsw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gphgmusqu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/ggjbahnjo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtiwnrlav.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/guvtfrvpn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gmqcwvvqg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gblwlybai.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gneuncngi.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gvhaygxtb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gexdwnnma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gzkdajczt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gfnaoycue.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/glvzgonku.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ggoickefo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gfaurxiow.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gjzgqrnwx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gvxuajfjy.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gqrrbakyz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gbmbxkxyu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gudpdvihz.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbcvflhlw.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gczdftccm.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gqtpskdmb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gwqueohjk.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqomuyshy.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/guyvqvhye.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtuwukudg.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gyftkclho.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggdzkmwdc.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdbhzqzly.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gzldlyrxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gqzrundpr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmduqmumm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvmrqsakp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdmkpwnta.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gsxkovewk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gzgccuzhi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gczzlcrwb.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gluoazvnw.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gbmjmozcf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gkgvnadbo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/glexvkzwd.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/garzdaeyi.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gpjcfukxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmhpylyof.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gspqsqdgj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/glzafivco.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gwiloldcn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/guobqgvnm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpuoojrrl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gisnlnzuq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/godghcndf.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbchcdily.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gclujpfek.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdrmtya.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gyzrqrsfy.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gaxuycsfi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gqukvjyur.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/geurgqnen.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/grpjwivje.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gymzkgbuu.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ghirjlesh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gqqjkimwc.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkkasteog.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnkaqetgx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gmrcjomds.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gifdrmyic.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gvkuydygr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gwtkphcqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gjxlnhyru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gilkccdzl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gwrmkorir.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gsqcobgqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmfxmzqgr.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gpztvfhgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/guhqveywl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gacyoeatn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gynrqvnbc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvudondhc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gaebmiohs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gkeqpuvlb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guondmwib.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtaftxjrb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gzvfvxiuj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gpyexmvrv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gxgxowdgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqtpqrzru.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gfqaeoxfl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gjdqjielq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/glxeeubzx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/glbfqgqow.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gituiybbq.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gpwvsmwzf.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gldrplrtn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/grutisojj.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/grvjtlwxs.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/glwmjjhgo.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gyejyctib.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gfsxnbtcb.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gkotszcmd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gvydpmcxt.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/giogqdxkh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gxjlsxfcy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gmrzrtrxx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gpkperzay.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ghtvhpdhs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gnulxnknx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gzeixenho.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gxnxhyqui.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gxjvjkhic.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gcqrdwzsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gmyzdyzns.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gthpagzxo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghgqfetlw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxjjayjyy.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnpkcenfp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gljagkbkz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnybqaect.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gxhsqshfr.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gfmwxkwwb.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gjaiuwdyo.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/guvhiifvd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gsqofzmgc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfzprkxol.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/glbriokie.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gswivztay.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwaleaa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gpmvemaxk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gtxzoyyqo.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqldbefvl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/grgkzyrsi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gikxfmqma.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/glsedpyqt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gsxgeqztx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gtlbijzdm.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gxkfxfpps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ggnhlqavw.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gdakafslt.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gudbgbzbx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/geajaureq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gifrilcyf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxathswlr.sHtML


<!-- 参考信息 -->