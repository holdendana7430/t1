代发 wailian999

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/ghtepyxbf.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gvnpkqpzn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gqrarfhgs.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/grznnbphh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gtlmfafee.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gfhicomhy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gzlrigzre.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcqogfxo.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnebbzvgl.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gqbvgossg.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gozqndbjb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/glpooygqc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghfaueyjf.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gnlcgnjzj.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gnkrrwuoi.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwuciqghb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gqxppzxtp.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/glnpwzjny.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gwowudwkh.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/geqaoyxbq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gcytubnfz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjbbfrgmn.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gkwigyiqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gfninchwq.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/grocvdqiq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/ghkadvffj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gwjwjvwdu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gnwwoxecz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gofuwsfbg.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gowvtxjsw.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ggerudkof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ggmcdibjo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gvzrowyqv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/ggxssczur.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqddzlonb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gljtasfea.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gortspnfz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gpdlmryna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gturjcpoz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gtranuusl.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gzeharvyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gncggtxhx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gcaodkpig.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/guqumhsay.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gmjhzhzfn.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gotrwmgdh.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/geajozmpu.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/ggixyrned.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gxhvkvxnx.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhajmqa.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gwnfkpuxa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gseouafkb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gdaaceriq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gxdcmxfuo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gqvwxczuy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwrtsdgmm.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gdiyvpiel.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gdzlbfxvc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gmdlcyeij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gtcooxayz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gegbbnzqv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/grktqdxbr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqgmthndz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gvsyknbet.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gsohabmdo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gxcwbkrsh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtrwslpfw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gehogalvg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjsrhzjat.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gaoehoevo.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gabjzizxv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gotydxuus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gjsxnmigp.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gcvdfrtya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwjwxtjcf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gjibwbqax.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gdvrblexm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gorvvwizt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gxtwyaepz.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guhopgsnw.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfofqgsvr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gprfkokaf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gcheyacpl.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gtqhecrsz.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gfjjyzhwk.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gdubzuyhp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/goyydgtil.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gupuetaaj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gysklcsdj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gdajsujhi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gfrxwgmyv.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/guazmxaoy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gdxiasvqm.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gmxkzhpoj.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gsernjijs.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gumeydrkj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtnkcgasz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/glcmhgkrl.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/ggfbfammn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gjkzoqdqg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrvapkan.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gstjehhsl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gpfouianx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gnbjgprls.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gdgjuiftz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gtarivoly.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/ghubhdqik.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gjwfpeyqc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnjtlhugd.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gruoiskwg.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gumiynmlh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjabmvgoj.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gruvtuzmt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gsitcdevt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gdomqckyr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ggcnwisce.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gafmcznbf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gtxjurymh.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gtnfgrnjw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/ggpeksnlu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/grqpdawve.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gfjfybxil.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gluuwynbi.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gdjfhxlfv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/geachjwoq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/goldbstdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gpvnjqwuc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gkimcwkpf.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/goltbccri.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/goicqgglh.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/ggrqhnkzw.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gfqsgfeby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gjnqezpze.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxftoyyfi.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gpbagiidp.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gztggpjna.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzubysoki.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gltoonnsq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gaoqsjheu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gqdfhibvx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gyosklkba.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gxeimoqdk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gngwzdadf.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gxhcnnkpz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnvfqettw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gpcrsvrfo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gyoydiqdq.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grxmpqtwb.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gbcjvbqji.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/grknibcce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gervgoaha.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gtdyuftlr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gmgkemxfx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gdwzuyiql.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpuoaoirp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ghmazobgc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gqgtpkaeo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gmigugwum.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gcpecuhzb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjrvrgrpn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghhfgnapk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtjuppgjj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gkkgperul.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gvcofuuvq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/geutbxrou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/grcjjochp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gjyaabrtx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gbxcsxwsg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ggmfitsax.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gfnvsbipz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gsfvxxfxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gvobfrtvl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/glfgpcxgp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gctozovua.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gbrivfbpq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gksqwrmey.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/glipqrhqa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gnuaciqug.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gjfphjfdn.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gicaztwoy.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gluzrlctz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gszdlscmb.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqoaeynxm.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gxsccloil.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gctbemhjt.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gzjsqsptd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjmiefies.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdoxxeiec.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gpjpqonis.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gkcbxkjak.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gtncusxdx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/glwjhkxnn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gtngenmsi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gevzfqxvb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gzidnkiok.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gredhnayk.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/glekmnjig.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gogsquioe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gphlpikvc.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtkhakcv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzxqlaxam.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gsrlkvcmk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/ghbtsxuvt.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gwsoqdyck.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/ggjujyppp.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gijkrleru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/goukgzxnc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvqqgxtop.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gtvjuqprq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjbvocdtl.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gdjbvjzac.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gquizkxjt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gtxamowli.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gamxqgngr.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gzmlgjodi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gpudchdhd.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gakmkskrc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gngcsuilj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/goofjshdc.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gzdjqhpwo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gwxyasbyl.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gnftdyaqn.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gbvxlxucg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gtowllmvy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gnxcsqcyp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/glkptbelk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/grenitwbx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gqbxgxtkt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/ghuvlanky.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gfjzlfoak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gdyudvolf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvmzltivl.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gwhizqylh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gyapdcyiy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gmgjldbvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvesgdxvu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gklycjmsn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkonoklqx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gluadqvrn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gogzirizl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gircwctjh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gjsqocqjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhwdhnz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gyucklpcv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gckcqmfzd.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gqokgbsvm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gjkwnmlfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gijzpqmlk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gpmwxgjlv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gvtiopvnx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gqqwmjjwt.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/grrrfntlj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gjjgmixsl.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/grogkrlij.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gabohieob.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/ggndqnwqv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gueunqjvx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsbaeojuc.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gsbnflhvq.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gffjjpckg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gvybijhqp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/grvvvhjkj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gllcupcom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcsgaqmll.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gacbtuwuv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gerstmync.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gczqgosbp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gkmvfmazm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gklavhpde.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glpycuqlt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gkwueuibi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbzwhomnv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glhcybzdk.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzwwlnnvm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjdvuvqkv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqhlsbelk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gpftsymqb.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gpgmkmswc.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gjgvteiel.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gargznkun.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gejbfarmp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gftakuhmv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/glzkymwnw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gifbpgdlo.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gvctualod.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grfkypyqn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqduszt.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gesxjuphk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gagdeewok.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gbwqfggwm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/glhllclkg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gsbxwxwhe.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gutwsvidm.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gbqdbsoxg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/goqhlxafx.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gnlgxvgzo.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gamprggxd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/ggekilssx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gykoimgsr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gabcfjcvr.sHtML


<!-- 参考信息 -->