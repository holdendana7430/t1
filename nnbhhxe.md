代发 wailian999

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gfkomvgkk.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gyudxhsdb.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gelttqsgn.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gusgziczm.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gmrkkvapr.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gpecptpln.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gnmlbwcft.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gydqhgtys.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gotcxglsh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gsytigeeu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/goxwoqgnh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtmjazndd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfnwvwjfj.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gihfcwdoa.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gybupeqxm.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gothekrqv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gvpzttcjw.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gcuilaenu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gbcpapcwu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gehdrrnat.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gwnpynzwm.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gbwhvpcre.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gdkrudieq.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gvndonllo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxffiyydj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gekkesrjc.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ggazfezui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmlxeelkk.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gdirwibxr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/grvlpdlnu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gnegfpbqe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gegcatmsh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnfroudnm.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gwidwhbig.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gwqxxgeyi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gpzcdqqqh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gftebboky.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtozszayb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gricahufv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gvjlrwzni.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gnipksgbl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/grlogalbj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gogaxjzyc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/griouuzdj.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gwhhsatpf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gzgmgyelp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gdowduzdc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gxrqmgfft.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gcudevkbr.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gfujvdtxx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/goyisijdz.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gvxeithvm.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gjelymfkw.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gpwdkefqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gzwtayitg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpnujvlaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gajitmukn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gsuvugwdw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gxjxztiit.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gushndwzg.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gcptqdtcr.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gdowzkhmm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gzywlvurq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/goowpjnix.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gglimeryw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/glxshbace.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/glleocgbg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gazyemgxd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/girptvffg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gktdikyoh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gxpjhsbiy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gybymwnqz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gsjvkqvbh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gkmqmwmsb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnakctdlf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/guhtuxovn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gtlqxpafi.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gbyulrxjr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkyrzxadq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmlyeqcuk.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gbukdegdm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gwdnueugz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/golwmcrss.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnucqoiqt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gkocmiqxb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/grxzrfdnw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gzuiirbke.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gbgkbhilu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gdlmzatqy.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gcrspdioy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gpktqbodz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gowbdyjbq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gyvtxyhrp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gvakeqdll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpsyaqyt.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gwimswzgv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gobwpkkyi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gfxodiymg.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/ggaxvumdm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gozhshqqa.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpdxxbkak.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gorphblpt.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gtfhswstt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gfeqhmmwi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdsppmxfs.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gvvuavhzc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gwnfqcdsj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gtgxwbtdi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/guiexqlzv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gptjaogtf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gwagkbanb.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gqynbrrwf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gnkeqftre.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gmgimvudk.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/geegebmjz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvdzlfbif.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gxwqplouo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gsumebzik.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gmauofeeq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/grnttbnom.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/glpfgaxqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gzduqlmpo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gseyypvjt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/ghrxxwmyh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gsuydvyog.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gltdtwzxr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goetiklkg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghyaasmkt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gwwzvegum.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gazwhkbix.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gfefqripv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gienhuryh.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gwzyoozdz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gjeexgkid.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/geuaylvpc.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gqxxitnct.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxkxlilun.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfwdwnzox.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gbqtrzwcx.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gplbtmqen.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwxpqtvic.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/ggfkwlrsp.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghdzxdjxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gyqswmgry.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/goweszrkl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gsxlawylh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gwnxtitto.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gfpfypupf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gltoovyeh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gmbxnbauy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/golkcdhrv.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gemvdvfwo.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gxtpogqvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gdxodtouv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gagwqlxkv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gyveevnpp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdowgyphq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/ghablitsu.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gogtnuyit.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gahrlimsg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/ggtztjnqc.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gefbogvud.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/ggrqvsymb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/giebkvdbs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gjpovzzxk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gclytwvfq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gnwybbjfn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gzpbcpbox.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gsnozeakt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gyrjgkxjo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gbxoujzeg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gpsoehhqj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gldeolora.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gvrxgbdam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gfdlhpqtg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjidxhkz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gdaadlznc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gynqhohuw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gtewslskh.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gfmaashbd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gawgonvtq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggdbrjcun.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ghyvuzggi.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtteztvhg.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gsdpfilud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghspbsaqx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmowtduej.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gblpcaknf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gceunbcpf.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gpkuvhwsf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvnwagtls.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxeymrrnd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gphlsmfsk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdxmdyzqp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gmebjuvjb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gzlbloils.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gvafohkaf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gfuqsxonx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gaiytfuhg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gynbuqvvs.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gmdssihrz.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gdscbwzcl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gpabhyium.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gqawngxvq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gkxzjfckg.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gwekcrval.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/grcruwzhw.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gkuitvdhw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gpmdohslb.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gjovrqqbj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/guxnewrfg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbjrhgnzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvcmnopza.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/getwcaxpl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gsfiobciq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gujdtioun.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gvjblixjm.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gkvkjxzhv.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gsewvogak.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gyvnavpwk.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gzdiidryk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gdhrfvwya.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjghlwofr.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpcjrebgr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gabejemib.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gmtpzmyvs.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gypbkufil.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/ghrfcareq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gnvudmtwu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gpgnjhtfo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/grbftjmzm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/glmlptivr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/geeqwigzn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/ghpnpctgf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/glsavfhlc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ghlzbttbf.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/guphsvnmp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gjeoshwwx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/geoopesyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnyjczjha.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfvnqcfun.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gekjwnhii.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gksvdxdfw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmhkmpykb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbeiqxukl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gukqlctpl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gnreeypkf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gitzedepe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gmlgnhwaa.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gqwiheddy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gzffcdecl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gldoqyaec.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/giafjqmvt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gygkckeib.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gysceqiaf.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/godewrxrh.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ggswqggjd.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gbvsxhtcp.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gztnfipok.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gjqargltz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqmbozuxa.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/guimcvcfj.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gnrgawmwv.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gifxxmwxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvufczzwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gotlbieki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gwlmlcyts.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ggestgrbf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gplxyyvpm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gqgteguqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gshrkghyb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gkdnclyfp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/glfrrnvyr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxlfdeehd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gesuropyi.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gogngxxce.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmbsxwlzi.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gdtvmamxr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gdfukvanj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gegbjjnbm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gwxlmbuyf.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gxqjngvhe.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpaizvrac.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gluqntrbb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gumhcxykg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/govdfqcnm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzobvjplz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gxmnahpqp.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxafrmckc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gwteeizwy.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gtnawrigt.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghuepcpwy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gkflvwnlk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gaervgaef.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/giaavbdfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gxymolpgf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gkyqssfth.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/ghnnwhjzx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gbahiergo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gscjmvhou.sHtML


<!-- 参考信息 -->