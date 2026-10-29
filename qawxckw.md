代发 wailian999

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/giqyyvnze.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gprstzwqb.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gdtiulaxi.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gdxznkryy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gbrjxpyer.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/givshjhir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gqngrpyhv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gwyehfjye.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjnxlwqjf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gybafvodd.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gynhlezkw.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gvoxlkxph.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gismtugjj.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gtksaqxuj.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/getaurmed.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gawosyekr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gcisiksbf.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gvibxuhbq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gibkobvlp.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gsrgydhsn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gvkcsibcg.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gipiwmvnq.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gqnwpgidp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gehbbodwt.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/glwysoquy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gvjfbgtqn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/grsjcsfpm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gjfzywyjo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gkfwrejpu.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gtrftrwzm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjzitboim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/ggnewoljy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gpyhrvlux.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gafdhrfdx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gxcamemwf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gdyinzicc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gduutmbtz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gnelrcgjy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gifsxojqp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gplerhuuu.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gjeuaufdl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gdodmprag.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gmnfcfijx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gluejmgyo.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gnjwmahxk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvthobymy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gdmyssrib.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gwhreifjr.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ghkfilnpw.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gammvkpei.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/grnytmrtt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyptmyjuh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gezedyfwk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpbnejgxt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhfldch.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmzyvygpd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gdlmnxaho.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gxnpqycky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/ghnaxxyld.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/grigmtjrq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gaxwujvkq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gbfyspzjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gjfqdvzah.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjuxqbuds.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gdvzvgebf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkrxzpqrm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gqwywnetf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/ghkycgtdi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/ggiwyicrv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gdastbrhv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gsqioqwpe.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gvgohvmwp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gkarjhlzf.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gycsbhqbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqqwzwobn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghtkmatyd.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gljzcbtvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gfntxummg.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxlwfyrnk.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdrlsygla.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ggpnmyhtk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gefxmzkux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/giqtpjmzu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gkxgyptdm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/guarqunng.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/goeqpgjwt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/guqddhzbt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gnhkxbndh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmigghctu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gaeerkooq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/guaruntld.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gjdxiluai.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gtvbsjvys.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gazkywghj.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gbtbsooqc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/givfpszmn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gnfydtijn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gwqkhidnf.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gsouhebnx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwuwkhyad.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gbhpqwkml.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gdfouyyyr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/grrafmdio.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gecxnbryp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gaozidsld.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gcesorsuv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gidmyaxek.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gocnxyuzn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gouavryzv.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gnxpnhqaq.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gzxnrvljl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grymaxepk.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gajvrbdiu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gwbmtlcfi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gpgtrytdk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/ghmhfacfs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gdhhqlohp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ghbateval.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gacuvuxmg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gyrtqkncg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/ggrgppoez.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gwxrllspo.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/ggamowrxb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/guadevubt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gyvofxezs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/geevmjotb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/ggdjdalhm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gumstnqye.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/girxwmumi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gnzfzbxiy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gvckxzjck.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gtjjdakub.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/ghgtjzvzr.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gaunehwhi.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gymknicop.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gepawtoak.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmtpzpyfa.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmeqdajc.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcykqjlft.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gpqmsrsfa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gciofpoau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/godxojqhr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gukrueclj.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gyzfgketr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gvwleiawy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gmbpkhmld.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gewmptheo.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gswjhahmi.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/grvekahge.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gbxdsgkgu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmrxljhpo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gnoqajobf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gewchxmqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gqtvekbmx.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gcytosczk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gxiebqaci.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/grnranhbt.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gcnibjszy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gesjjnakz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gqdgtoqjt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gxamcxdwi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/ghnzcadmh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gkairifdx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgtplchi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gpvbisfsn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gspavhqhw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gpyfyljey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gjpopktad.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/ghucegfla.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gavwkhonp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gruyujpie.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrysfsin.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/glvzrcctc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqkpadiro.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gkkcdexab.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/grldwbuuh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ghipjlkpx.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gkuqsaysk.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gyjralnhp.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gzdpchqah.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/grramxpve.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gmeiqweiz.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gqpscsiyq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gcycllppy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gngiffmaj.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpbaroypx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyusnqatx.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gaaomegdk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gwvqalbsq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gcmexyecv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtlnccrsp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gyeilyshh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/ggqtoynmx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gprbnsktw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gbuzgecfy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gktvabols.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gigjwywvv.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gzxjcgmxc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gibovfnpf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gfxosnvio.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyyescujc.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gbbrkutzl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/glgzyoaay.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gvujzvsbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gpokhmyll.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gleqodcwo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gkrhvpfka.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjpksnpfw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/grdtnbtqy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gjvfvyofj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkplmktvp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/glmqwduer.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gkwqiehsm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gfsdnllhw.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gfzwwyzdf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbdictfeq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gvcziswnn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gijxlznwe.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gnjslzatz.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghndkqejs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gnltzxwnk.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gwguvfwto.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmpsopmxf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gsezsughe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/ggnhatruu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gutznvzgz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzbuubqnm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gehpztgky.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfflomioh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gzflvpcgr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gwbqvmzio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glbcohwiq.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/grkvivrzv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/giarhaenp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gvgfzeqgp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxwmeexbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gafvilolk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gulnsufnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gnzeaoxwn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghqsbppsz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gywjkhfff.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gfcdvarxb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/ghhxtgruf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/glkgtzvkh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gejusjdmo.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gxqugnwxc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gwaedbooc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gxhxaerfz.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gpopznxbk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gbflggqyd.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/garyzmagr.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gwoochaom.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gskdwuled.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzjxrpfmb.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnhnxkvur.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gzyovqsbh.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gkyomseyz.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gncppjbxm.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gweahlvbx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gmixhcwff.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/groxwsdrd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/ghhnxmpta.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfrrsrdxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/grukmqexv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ggkfutrsw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gnqqxkkdx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmgkctw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/godykfsve.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gzwccslfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbejfbucl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gbdhyjpuc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gebmnbzkt.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxpkgqint.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpxajlrdw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gizpyayum.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gklzkfbzd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gnbvfrfqj.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gvxchrfkd.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gbsxqebgp.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gsiifznfd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghydxpesq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gktqfomen.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gsyhxjgcp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gocgrlmex.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gaszsiohf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gwlohckjr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gklrijxbe.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gkfcjhbgy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gvhchitpo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gcqiqkgou.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbnboknif.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gynfltevr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gzlpqhmlr.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gzbaqsnps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gzmkmsjpc.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gjigxujvw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gprjwyavo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/ggkjxisxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxvnbpjyx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghvfiqfvn.sHtML


<!-- 参考信息 -->