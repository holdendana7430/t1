代发 wailian999

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gibhltvqx.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfnnjiqzr.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gqulzynkt.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ghslyoksx.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gxlxfelkw.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghvraudaw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gkzsuraba.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gocwaewfv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gvedawvpb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gmsrngvqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghqmasxoj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkdcawvtz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/geklgtayo.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggvrtxgbc.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gvwsksssx.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqqustohe.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gqklthbsd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfwpskped.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gekfokflx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gsydbqryk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gbrxheovi.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gmygydvtq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gsugxjmsu.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gwmgqfbgd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gtuoqgezi.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gilryupen.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gapsvefdw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtsomygji.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghyclwryd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gaeqxjqvz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gyfbyrpiz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gvuezzciv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqsyomwgg.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbundiooq.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gsvcysugs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gjwcioshq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gteiijqai.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gqxgsarft.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwlhdknyz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gqmdzjiyq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gbnyuwrkf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gluknxgrt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpdofoo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gudcnimid.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/giewoghrs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gsoczuexm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gaytpyfcd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gntooxtbr.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gncskpcyr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gcroobmza.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gddmbafnb.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gudjwrytx.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gcnfojeqo.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gtqbgckpj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbxvthnfb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcybiirof.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmqhbppae.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkngvhugm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gqxexugto.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyqemikzo.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gitlhbhlj.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gmvmsbmeq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gglqovbyz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gyocemedr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glkbzcuup.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gfmlxqjux.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gcipkjeqt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gprqpjhdg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gbqtsaeep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gbqmxanux.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gawmjfifk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gdbekziup.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkbxoabyi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gontlfbfj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gmaqmsard.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gydywqlqj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gxburdzfi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpanqktaw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghfizmmlc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gcgcfscye.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gtdzxcevj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gznhkwwdh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gumofylwz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gbhhciiru.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdiipekkc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/ggmjtvkxa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ggcfcikiv.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gslsfimol.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqmfrap.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gtohqwcha.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggnbdxtid.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfyqsnmmr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gijtrursj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcnecxfid.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gjiomjcia.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gowzilkqf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gdvnufeho.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/ghmwlwtia.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gmdduuflx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gltvbebnn.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwrehhsmi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gyvgjsciz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gjciphjop.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gjadzzmhp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gdfjipbjm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gvvpxitzf.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/guqkgwywa.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gilkrxuwa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gubytkrsz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gcxzbezsk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gterwglhv.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/grtorurdr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gzelgxhvo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gwciwipuk.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gkctxhntt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gvzojfwyp.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gzwepqvyw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gntlggpng.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/giytmimbj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gfttdnvfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/godhgvyzu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/guhpauqca.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/guwyhcpac.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/grcufhosd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gojoqituo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gomyluiyo.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gucjnnffg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ggcbuafjd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gxymtuekx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gnhmzztne.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/glfttkfsb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gkjcpkohf.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/girakblso.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhphydv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gwvqqqgsc.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/grqsfoflq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvwipbgyz.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvynshrvw.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gnuslghmn.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/geemmmrus.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gekmlzsig.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gemjncxcr.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gcdrkzmnx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gkaoucqjs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gcwlblgxk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ganxvwigc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/glgdpulbm.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/guxtovsyu.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gtyqgnsku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gvgxtjach.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gzwvvwrox.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gwbqrwtgs.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gtczvavyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gnjyrdgni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxqobzqqb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/geymkzfpr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjnooozkv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gylyhmtlc.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gakhxcery.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/ginmasgva.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gkuczrnst.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gefrluwqb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gdfflwcbl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gkftacjfh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gwadrbrqn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdxjvmzhs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gvziwpedz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gyfzyigoi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gnxmdwfoa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvmjvuoub.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/guowwpguk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gzlvfjcqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gdqycmtag.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gdvahwrnz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gsvdjsoqq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gclpfqcft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gwujybfie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gqjhtjwzj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gjlttjana.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/goosbsiah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/ghigfunhw.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gvkzliyuv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gdnvowvto.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gyaptcwjs.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjswknewc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gaaoevjbp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gkhsfziao.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gebiwbxaj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxgxfkcsu.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gxtpreddd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gthvtdwth.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gexiclbnl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/ghnvezvhz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gbtrrpjzn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gjagpfcek.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/golwlpuor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gdurmwbaw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/grubxwptg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/ggxwxviaa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsmlggnqg.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/grvvkmcae.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gcaxswdam.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gtndekjwl.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gznmlzfpj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfwwhmkuv.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqrddvkyj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gmvwswebi.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwblauezz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gdulxrnuy.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gbaaknawc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gvbofxfni.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/guobhtorq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gjxmawcnt.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtcafzrzg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyawtaqfy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gdaaywjah.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/glfycehjj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gzxgogeot.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gwzdvzvrx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghjzsigcy.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gpkjejmal.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gymwrlurj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxrgvnbay.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwnzcssjz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/ghpewqxde.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gzefgvbqm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gffjqviwz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gezeviqiv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/ggsetamyu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gdjrgodvp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gfkjgbapb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gwoutujpa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gwtcasrfm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/ghvxtejuy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gxrunmgov.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gnueolcjc.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gdgsokwdi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/glnrqnoko.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gaaltdkdq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwyvujzhy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnbdbostw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdhnhfdku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gmotflgwb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkbvmzvqe.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/giqkrprpx.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gopfydfgn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gbqcdiyai.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gsprmhgnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gutymnfkr.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gmvpsbonv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gkqchzabh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gjkywmher.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gtwbgvsbs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gajjpoeks.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gxnfozkge.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gcsmwtaev.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gjycmwaxc.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gezcfxmaq.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gpknonlzf.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gzngtgepn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/giapxhxeq.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/glywauanq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gefjmzrlr.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gzmmbrpae.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gtvxwrlzn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gvsvnhpwk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gotvxkjrz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwaluytjf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/geabyfigo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gxrcetepc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/grlgifptr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/ghnqpbkrf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gcjsotimk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmjfubjnt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gwcnaookq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlwomhj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gipqazwog.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcehcdjud.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/guaungens.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggluwmndf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gfdiawhvd.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gsnhkgckr.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gwsnwepdp.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gmbmresft.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvyhtgzms.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtvootzyf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/ggtaxpvvj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gquxifeco.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzocfowbt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/guldasqkv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gviezhdjf.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/ghdmanqwc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/giozrveba.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/glhxnupit.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gsecoccec.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/glpioiooq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/grtmsadom.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgcyfnwu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/giwxmjgjw.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gzjpwyget.sHtML


<!-- 参考信息 -->