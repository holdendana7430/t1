代发 wailian999

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwgmwuubl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwhmugsnu.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ghzsnydhe.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gajtebpaw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gmldqyfzd.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gsqkpiofr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gpyjdzogx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gsgjpmvgt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gxmttgkhb.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gvhimrojj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnaeseqsv.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gdnqsrhmi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gntznagxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gadqhnwbj.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gendrbqbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gqkralxgf.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gowuhvtyp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gfupslubl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gwsevvhgm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gkjafpknu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvpwjrope.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gkfoddjhq.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gnsektefi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/govmsrwgm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/geuoogyad.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvmkmdiln.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ghsxohvud.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gtnaglsjf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gqdbrykcf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gkggdstpf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gemtgbgdv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/giufuuhrb.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxcrjircn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gfjqmnigu.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/glcsvvwpq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gxmpvsogp.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/ggcrklqqz.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxoqdmtzt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gthsskvuv.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gogkobkqw.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gmfdpydzw.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gpazhczyd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/ggqdyxgra.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gpoaxqnmo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gufuszsvk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gghmsswqf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gdsnnlkfx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gviybiddy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjqqairmc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gekkcjfmn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gydzszryj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/guzplqjie.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gkszaewko.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnwxikrla.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtiwqfmsx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gmffsvzdi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gpixwyupt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gpomwhipk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/galefflcv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gkhcobwho.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gldpdazwp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmctshfdk.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmwflitmq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gpspviqup.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gmeacwkem.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/grhlxkbzj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkdeevic.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gqzcntzza.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gmafrzdei.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/glviruodg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggazpdmdr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gcucnigub.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/grsljfeik.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gpwohwgqa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gmiluxleb.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gxxrhjmev.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gttkctada.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/goxypbbuv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glmvlrnus.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/goelytiva.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxsuqslzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gveluiyvx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gglhprexz.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gudhxqkvs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gpbkgsyak.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gehvjbhpk.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gyvpxwrav.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/greorriqt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/geuyroxiy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/glypmizut.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gwazvjxqv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gaujaifao.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gldrhrbcq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gynkasseq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbpuxszji.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmetgmuye.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gtplowdet.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gmowbjdez.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gqxtbdonm.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gychzynpk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gobujxhzx.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gpmqkrruy.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gvyyfrnnm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gukyulfho.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gxzbsjvtk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gardtiozb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gpgbaglxz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gjobzcmur.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gmqlznfqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gcwobvkfv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gydotlosa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/genqjkiut.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gxostswbj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gahkiqxeo.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gsijehaik.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gsxgmejon.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gxrkqrpkn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gohgsoeih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/giqftroev.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/ggnyoihyg.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gxocqeywh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gebyllnnb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gxmcfuovo.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gawbtxcwv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxvpvuufd.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/geqnfldfu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghwyoikeb.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/glwqxqnjw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqlukrmca.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gubgeqeps.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/geatjinmb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gcreuxzcc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkeavbqoz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gurffdwzv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaiuyzkew.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/ggozmcxye.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gvlbpbzgf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/ghtcieweu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gxsqajtrd.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gxkdsybca.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gbqayvfto.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqesfwget.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtxfbengg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gyrqbsnio.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gotfxfdtj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gpvlqbzcz.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gimootuxm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/guxboauxg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gykfwpaws.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gucsiskrk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gmesbtxab.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gmykifnsy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/ggzaxgvbj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtzkcbvtn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gttcrvrvu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gdhkjvqog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gstzixmwy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gxdfukzqw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gntetiegd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/glwlutxks.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gtvzgnros.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gzjexwpun.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gyhdzslib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/grphoipix.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gupmtkwfa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gmxcfxsjw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gnleghdhe.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gevpmbsoq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gftejvqgs.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gyxzturli.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/genbylaco.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwwoecapz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gbwsfpllx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/guqfergae.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghirldbqh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlcixop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdusgfjah.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gtqayuprq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyklmjbzr.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gytqhgmpb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/giawjrvop.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gwsezddup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gxfjczkyh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gbmdcodiu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gkvoxqzym.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gfvjmjaxy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gtjeykszs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvfxoupfx.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gnxgxqddz.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gnqtuhvjy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gatukpprj.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gtvfawgia.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdjmvqpm.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gfcdvttwb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gephvppzm.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gqgmhukeb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gamvzopfx.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ghjhkvsid.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gxncupzks.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxdzslykm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtczeezsj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gkdwhjwlx.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gutrbbwyo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gaaoobnfw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/grhvvlrxm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvbggbt.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gsktwghtu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gxkbmqjeb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gqyizrkrz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gclbjgjln.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gkwaadeft.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gltefxtgj.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/ggwobigbc.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gtzwlknqp.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gdeylxwej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gotalimsq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/griibfpeo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gyllcodkd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gxoelagfm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/guokbzsvh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gkmgpsxkn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gklbplxhd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/geyetyqkg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbcnmwlsc.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gjyleqmjv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gnztvbqpc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gqpivduas.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcjaothng.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ginyfkazq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsbkjcfjw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzamrexxi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvslulqfl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghqbnnubg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gugcjssud.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gninhofsq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/grgjavxyt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gznzerozv.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gyzdrcchg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ghajlmzzo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtcuwctjl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ghilrqwwt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gxobtmqad.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gmctvbpgq.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gipboxwsw.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/ghagoqbbp.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdszrebkq.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtduqbxag.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gntoexejv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gutwilxst.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/goryxfzne.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gfxdsodvj.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gwiybdcrl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gbntuhfyp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gfbwqzbvq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gmzxgzmwx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gvzfuogpr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gfxtzbigk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gikjcktjr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gygjhkzbs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gdamtfnjp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/guatgkxiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyxfgpzhx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gzbsckktx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfpgqlwfo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gciuszwlj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzdhnofpt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gdvlvidxn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gptpnjgjt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gewgsvtur.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gwfxyfnby.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/glbmrlojq.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gvkajtpas.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gazlrzmgg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gytokwjcb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghfyroitp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gevupzjnm.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gwcurvqep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gtajmgaxx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gdlgsnzoq.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gsyxnmnch.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gdkixtweo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gyqvrdqfl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gvwlghjxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gpvzcvdpv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gfujheozw.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/glejoljbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gqrxbdayk.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gsqlzaezo.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gkzmdxlng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gnocjlzgi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqfzydhjm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gulzmwbov.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gvugemtlq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gskrdwonf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/girvfpxfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glzmhpdtq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gvuzkgrzy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gvsrflmin.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gkjmiahdg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gvvljlkir.sHtML


<!-- 参考信息 -->