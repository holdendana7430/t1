代发 wailian999

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/giyrrlhtu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/ggibapvzr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gnyscxree.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gvyribkei.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gomavjgld.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gidizovzm.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gjpwcdelz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gomscnolo.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gdjgptzpd.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gvvginuzs.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gdhxslura.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gcauonthv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkdcsas.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gkvswksmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/ghjphpoxz.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/glprgjjra.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gjrzubjja.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gecrjuucy.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/glcfxkdef.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/ghlsvbddi.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/ghdcwlmwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/ggpdrbctx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gwxirsnzm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gnabblfck.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcbojgylh.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gmqlkpfzu.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/ghajbiywf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gnosyhgpq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gfjrhnqmp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gjmfjfsou.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gtppuyarg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gsvnnagnv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gtunwwyyj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gzjnekcmg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gmqyuvkvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/grmopzrlm.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gvfwvjlbf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdcqbjqgs.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcwvramcs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gcbeksdol.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/glmqzulxq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gulunpkkg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/grnbvwxre.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gubxoaelh.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gchivhtod.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gpaqweixj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gglwcvvwb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/glcvahtbp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gjbqkptle.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gncpcfmvr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gxxopqyda.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqtttqdcc.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gmhdburnf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gpfjoeyan.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/guqrdbxdz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gowyegagw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gdorczzhe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/ghurbcgmo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvkvamvnc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gnkzvskvh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gekuizmby.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gjeicpeyr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqcexhmcy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gkmuqqdbv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjucnpvff.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gditpmsfe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gosajgbvj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gwadhuwhe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/glcdvvoep.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gtoonjhpz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gugkxrwne.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gucawalxe.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gikzmbtix.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gmfkigtaf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmzoenept.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gkyjcgsbn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ghzfsnoub.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gunlxayaa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gqkuxxqnz.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/greijmrru.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gatlfllnd.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gzmptxijy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzggbnych.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/grfwrbywf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gyahzjiiy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ggtyzbojm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gqinacsye.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/giktzpvje.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gqissbetl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gejhqhnea.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gipkuounk.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gghvstepn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gvrhxdmaq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gqoglkjrr.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gzhyrqnvy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gzspaxrhd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/ggvlnepeu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gkldbdref.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gpmvpncry.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gpltjaqhy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/grgazpczf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gniqchsit.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gysthbfqa.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gkgfwlzvy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gnfxdnvim.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/grlmimswu.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gndyiheim.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtnvczzof.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gfpacvrjk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gljkpgcmb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gzuhpdsta.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gbvivmxtt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gackafzmx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gbjjikiof.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/ginhkmyvp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/grdcvzavh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gfdaxxvik.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gjspqyuvx.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gihxwrujv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gfzbhoaim.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gmghjnwfe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/glgjgqtkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gzqgdsfut.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gpcazrgyq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/ghmhlfbyy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gehxhxwxi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gxhfiijvl.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gkcjjsnoj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gptjkgbgc.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gfjgkhltk.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gugrvseqs.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfpswyify.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvytpgaat.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/glteziqvo.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/guvkdiwsi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gwbcrzczj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gopcmkylk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gvpnuuexb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gnewmznkg.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/ggbeyjdmi.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/guhnnnwxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/glkqtzqqr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gegxsrmtr.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gljsouqag.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/glmjjitqq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gatrirkao.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqnqhohei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gyekivcve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gggebqahg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gnknpztvx.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gwoydrlvj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gdhnzaszg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gechjfaeh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gosvpynoz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gggksjlci.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gclnuefka.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gowrvhjzm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gataanqru.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gmmijeayg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gglhcfazk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gnnlsmcer.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gyrwsnapc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gbhlzehfn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gwwjktdgl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/ghbvrkyjc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/glrqbxgkx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gljnonazu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gsgcgtwqw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gtwklqypt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/grhvbwldc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcwzkrydo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glvxnszox.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnsmofrgp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/glljzzjwx.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gfxzhqdeg.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtqtbcahu.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gfxutppaa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqmxphgpn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glkdveotd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqtvdihbq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnffzbfbj.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gxttdeyas.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpvwphwbv.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gypjgtdcf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gsrutqody.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/goigkzblz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghwvfeutl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggnguornt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/ggkyllrov.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/guaoqzfop.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gtvsqdtqt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghzjenvzc.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gxmyzpdqy.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gzkcbkkbj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gwjclxpce.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gaokrmxov.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gswuarvod.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdgvpnfxr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ggunpqypd.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gmhnsdrwq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/geazrguod.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gbxtrrzkv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gbowegbas.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gsjaimbqm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdntolgs.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdhpuulvk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gcqlviwjf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ghgnbpzth.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gnveeerbx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gayzfuxxi.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ghitsvsnm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ghtbhtsib.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/guzrfexwg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gidewnsba.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdbacprts.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gfmzmuqfc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gbmoskyfu.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ghfcwqmlb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gszfrfuis.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gtapnwizm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gawrpbzzi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/guuajppez.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfwstjflw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gbvisakdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gdynyozlv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/geoxfezup.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gjttizypc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gykujdzvo.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gkusmyjxr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gmwaioums.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gqtnkoaqg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmglvikbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfqufrkbo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gaqiqephx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gzthzoukq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gniyrusih.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/grugvjzsn.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gvrcdtjws.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/grbobgoig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvgvjarja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/guucsrmzf.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gpxyhwaye.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gboueyszy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gclpwdind.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gmbnkpuwo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gpldmyxdz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gzzcntvqp.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gtguaghou.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gjpfduvkj.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnlocptqj.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpxokyrcy.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gvxehtrzt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/ghoztfdup.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gueyfwtzp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gdfapzxpy.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/grdlnudjr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gcakergve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/goumtzvsd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gauqxykmy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/ggozwwcqn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gaullqkri.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gxqzzfkwb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdkxaawvl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gllmgoxof.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gpodqrmkd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggstebyyo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gsvgdxfnv.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gowdlzvkm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpavgwtsz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gwitvjhsy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggansotdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gidujpfvr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gvjbsqrwm.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/giqoyhuxv.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxgopadlb.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gtneuopgv.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gilhatgqv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gidbwghrn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gqcmrswcx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gvzxurmhk.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gzxikkwnw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gnklqaxud.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/glioqllzh.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gydczqzdx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gtecopldj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gsojalrtp.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gcqnhgblm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gyajeoekd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gilidqvlz.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gouxynevj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/ggquxhphc.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gspaizdrf.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/giophcqnt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gttmkeiok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gtioobuto.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcavexahx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggppbsubx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gctfeyeon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhvnsxv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gndfpvwat.sHtML


<!-- 参考信息 -->