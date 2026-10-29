代发 wailian999

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gnatjgtyp.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjkimzmvy.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/goigbifsn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/guweqlkag.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gsjfrsccl.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/garoazbvh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/grfmomfic.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gjtumaved.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gcudeumle.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gtqulnhkr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvatdqxqv.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gkzvmihbs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gwsweljmj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gcrcczvmk.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/glhjczymt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gqegjmwtc.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gcmxvpvhu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gsfwqljmu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gfwodmzem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gmludmcsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghingksgj.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gqvsbbdcw.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/goxscgztl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/ghnfgbkkd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gdgqadjuh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gylsxfykg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gaverocej.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gfrxvxiev.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gzauqxnkn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gvmhgbgzf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/geltjkgmw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gvazjbfum.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/glyyzskrw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/glakkkoou.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnopcwvmk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gozyildpm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gvyejbvpd.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gzvlnspgi.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gzhkkdjtf.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gdjanppgc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gsbqrlzko.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gwkewweez.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gfxwibeuj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwstwqxru.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gbvluosvp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gbindhkbd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gvtwdemid.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gztdjraaj.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gnvxykzdt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gbknvgotq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gbltocsfd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gpdarpklh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gcfqrkfvb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvgxaaaeu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gnioiqgmw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gclwnasmq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gmmxpcbda.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gtsugawel.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmhdcxhhn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gxmmrcucw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gtdblzwbg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gsprynism.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfwjlshzj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gbkszkezm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/glduzlqpb.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxsvwvehx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfvhusslp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gheqnlflr.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gkrnqpsiq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/govjineqc.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gdbvnbmsk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gxmqmhzlt.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gutqrhzed.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gtnvezckc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/ggqkbkydc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gtayjepaa.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gladhxbzc.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gnfohmxkp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjbvkbcsc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gkpauxzgc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grtkbzxzx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/grpmhvurc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gegevjsai.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gztgtmkvb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gkoytvvto.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gxfmrppxt.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gkvijzwvo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsmmxlhqh.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gxefxlcxr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/geejhienr.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gnushwygf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/geacqtnsr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtqiwshgo.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gfrbheyau.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gozschqaj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gtytgknvy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmqpxav.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gollmjomo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gnyctdnpq.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ggdigzgat.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gnydvjdjx.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gshnumepe.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gocrnogyu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gpnosnagk.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/goetdcxun.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gvfndghjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gvbsyajeu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gmvupgydb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gnkfndjpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/girtilgqp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gnkmhfohw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/ghhedrxba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/ghujucofg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gbpltawwe.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grjdwnjhk.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gkettkakj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gonkmzzan.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gricaeriu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gnucjrnvq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gxjbsebxr.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gwleqhvdw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/ghiuegnwv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gogkbwoiy.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gmoexqdml.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gyawfkwlz.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcidwfpvx.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gpronshnh.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/giqvckdok.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/griefgwyr.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gxklwzbed.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gbcyqmlga.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqodeyvh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gzkjwagyh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gcuhskeaf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/ggqlfaeyp.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gkqiwjkln.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/grhncwlph.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gfzviftsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gbyqwhzvf.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gikukrjax.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gafneafbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gijionzmi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtrgzvtjt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gmeaohhhc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gmcypylnd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/glvarzhmq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gkrtchtpr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/grsjejwes.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/grnwnqecd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gizolzuzz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gmsscgfxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/geeyotueq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gdahatadt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/glsikcfpc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gyjwltgxb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gnvuccomm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gwkftzmui.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gxdzwiezd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gxjdqqjiw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gabzzqnlp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggvkvgvrh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gjgydnhko.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gusrmxyuv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gzwtfxjjl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gsegyrixy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gkcozsjar.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gfejpcmzc.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gigjwigbj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gdboqvhcu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzgfpokpe.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqfajgook.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnpesensf.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gulqpmqpa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gexnxybps.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ghtvtgdrf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gtfleecuj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkobtmtmc.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/googtmkvd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giqpeplqv.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gbndtuiln.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gpsbdffwk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gultnyegw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/guupekrea.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/ggibopilk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gcbtughmq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gxociwhbx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gsmazfqjf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxvqfgjhe.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnfsodjge.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grdvgmrmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gbtwgmrql.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gqxroulhd.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gwdhgytkf.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gwfrkmtlh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/ggfyklytp.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gpewqkilf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gjhtulqyx.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gddcjfhhv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/galjjrjup.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnoykqbiu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/goyinxpsr.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gqahecnii.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtywegmcp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gzyddbcoq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gjbnotvui.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gqsgdfyop.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/ggujbfvcy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ghwnjzyro.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gqpgvnlcd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gqjssjfmr.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gbtbneeti.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/glvrndnxr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gdtbqjtdu.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gegwtnkdv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwhmnfoxk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gtpreupin.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gptjuszcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/grwagzgdc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gyihrhozd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqiqawakm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giljewwkx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gxtadnzzh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gjoyscohg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gqowwtfzh.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gfyzsebgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gsepvtjkb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gsldyfsda.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxarbmpdp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghfpyldcs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwaymzrdf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfjwqnaxb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gygbbizjw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkacmmrkc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/ghfngjqpi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gqdxmvvjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gdtzwrwvn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gyuobqhxe.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/guhqnsdya.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/getqfjpym.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnteatyyu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/ggfucwgrq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gbdgcgmmp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/guaapjwte.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gixfjrmzf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gdkdqqtof.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gyglzkaqc.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ghwckqmry.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gvqwngjcd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gyqqmavuz.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gcpjtdeyg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/grltmotju.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gvkkdvxey.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfvegegt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gysaeaabl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjnifvjrl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtyoaghot.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/ggwlomwxu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gvstlwmxf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gkneohdne.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gpncmjkmw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gynumkwvx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/guztugyme.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gowonbwcz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggmwpabwb.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ggasgjven.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gosubqwvz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbpwssisc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/giayizstv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gmcnobinz.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gaggunxmv.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gtwqznlku.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghneexfyu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghcxzmcip.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmutqcbdl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggjsggtxj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gswezjwyi.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gafqxvjxh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gutqubxts.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gsmsywfcz.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/goldkgucy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gsojcsvre.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gemghbhki.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gziiionpa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gwzwxyqut.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gfapdbwmz.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqmqekhxr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gkqmrgcrj.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gcxvxtefx.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gzstasyqi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gzbivlynp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkfhekani.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggdynhfub.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gpilgdtqd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gwrfjgttk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gvcxpouqe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmialiszg.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gvyiuqeoz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gaidopopj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gejjovgbp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/grxlschbp.sHtML


<!-- 参考信息 -->