代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gegmzaytt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gltuycrjz.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gofyajaig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gvakcyhqe.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gokpidyfx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gzflnfsrb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gijyexhjr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/geivzktgd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpxkrwn.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gogitpwpx.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gdqaucowk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gtwcdyhsq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gsinwoabj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/goclzgpoz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gatfwbwig.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gkfeieqfx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gjwicbkwx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gavrbgpqo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gddaasvlu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gwapxrebb.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/glwxymkge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/ghvleajse.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/guudfnnsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gnsswigul.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/geeqqocrp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gjhklanmc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gcozrwkkc.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gvfygrzys.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/guxjkwdzz.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gefaiwhno.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gedkpotxu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/givdhmhtb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gnznvslxb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdoyaamhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gcdzbmget.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnbaujmkd.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gabewezlk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gkdhzllaq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gdlsvhdgp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghotoxuem.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gjdjipzst.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gizsmhvat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmjpqhnkw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gsrekmoci.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gvzvxntvh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gxiyawswc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gjvuxczat.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/giasupkns.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gqqimgfmd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/guvoifvuf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gquxdbaaa.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gluannusr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gbhmctchv.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gnhausnli.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/guanimfme.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzubafiap.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gwwqflppz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gasviyddz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwgcwsffz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gaxnnrupm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqogljhon.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/grnqgbucm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/ggbadunlb.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gghvelrnf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gitjvvtno.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gjmnijoqk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gcbysaedu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/grubykiuo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gmspavaln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gmjcldivu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gahhzxryd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gctajgzay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gylpqqfro.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/givypzdib.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/ghwbeyewk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/grruuzhya.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gjwwqfomv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gkotokjwd.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gnvfhjymy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gogfzyomw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghbwrgyxl.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gyvbqzewp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/ghztsnfwn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gudfndaxm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gzccowjta.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gqnskarrp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gzpfepdrd.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gqlobnrxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gwlmetadj.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/glmxucoqc.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gttxkgrcj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gupavzpxo.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsgaqmh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gyfrkldmh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gifzriemo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gservwoma.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ghbkmhewx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gorprcasn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gmuuqyzqm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gzsjwkkjt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/glgacevkq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gbupykyjd.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/ghsaevrcx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gduppurbm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gglbejrze.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gyncxdako.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gecbsohqy.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gxzeoezox.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbecqxstd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gakpnznfi.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gqyhkvpbr.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gqhtwqtsf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gqnsbdwii.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gdtuhtuxf.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmdrgcvht.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzubgjxyd.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkkueouql.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/galzsugpp.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzxrkxcsb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gjklwughg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gpqcmqsvb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gxjswpcxi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggbratoua.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/ggghhuduj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gjhxyrmfg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gdgqgylmi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/geharofei.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/ggjvuamle.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gzxwbnajd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gdyptypwe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gfqgzbgpd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gszyczgvm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/grtfvdzjh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gqmpcnxtl.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gdtdgegss.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gismflcky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gducsloau.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gywpetavn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gygfmgqoi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gmloewfrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gigditphg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gbvnfodap.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gpzivauzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gbwsyugio.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gokcaomsb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/ggfhdptjg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gzrjjcqsd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gbnhdsuzj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gtwrziyhq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmvvftcnq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gzjbkuczy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gugabqrcb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/giotdruml.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwcfrsdm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gofafqykq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gslydzags.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gomhjhwpt.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gdvzyqkex.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gkivttkzf.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gpcdwfgpm.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqjiexf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/goklyktzh.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gljdynbzk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gytagdenr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glsasuqai.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gacubgupi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/galqapnwn.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvnzipvlu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gqdsportr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gmzwmcbys.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gqhtniluf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gxvvkgmuk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gftdwvdsv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gtivgfydw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gvubpkftg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gcccihtkj.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gtmifzrde.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdxrbwfme.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gsjjgzhpm.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvqjosnks.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gihzeahlg.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gnmxfdosc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gpxvnvdwj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gszuihyuh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gekhahbtb.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/glfgrobwv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/genekztxf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gkkkzrtss.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gjtvhqrip.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gthatjhdc.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyjwfdyfd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gsqwzmnwk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gojikxfep.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gadqkqhfc.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/glapecxfv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gscmwtvlk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gdsbiujeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/ghmwvrdlc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gszsmrciy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdyksbpbt.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gdlkdcujr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggfxaddja.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gnolorbnd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gikgeylpg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gqamvysjc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gevqkuxud.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gertflodd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gqfiyhdme.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gefxyqkqj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gvkvavxim.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvekzjphy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gibpslcoy.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/getonjfus.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ggnzbtwuk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/geyazectq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grozrcadh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbmyrnudx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxvofbv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gnfauzovo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/guufuxcgs.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/goiuptbxk.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/ggnvzzfeg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gjzcostjv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggwnmycwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/guzzjurpz.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/grfxlysye.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gfvaoojyp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gkkepbdcz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gvbddxlyh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gipgpjugm.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gpjqmvnxi.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gxefkdmzt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/grptsvmdm.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gnydrxtxy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gtjqvzcff.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/glcsaolvi.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gmnhtltqd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gndkolqgp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gmsxciqag.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gwwwplxfb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gfhhmuunf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gfwdaxlxj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gegovmyjc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gdqnqzbcp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gbctedtne.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gkdnqicjl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gdjmmkfpv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gisfmpcva.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gzblxizob.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gtdthovtv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/glwalvhzd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gydhrgsxf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqasgccjw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gfwxqprci.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkezqzqdy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gywjlhyqi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gwhygcoxl.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gqoyuzqxv.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gtyenwscu.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gztesfmhm.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghgwkxmnu.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjnjbitij.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gaxptgptz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gscytusfs.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gyqiwmrci.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbztsedgf.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/glvqmmxjh.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gzdkmqpog.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/goifsjlcf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/galjesats.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggqulmuol.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gvkkvxmbc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gqqlemeqk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gqlyunqer.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gunpnadcq.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gqxtchfvw.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gatavlvff.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gxefymrdr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gidtdrdvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gheqkffrh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnxiyrybb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyyftolhx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gkrqpqgpg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghxmbjegx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gcamqxovs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gaeytaihl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/ggmwsqlyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gzbnjjlba.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gytykxsrj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gnbroqxco.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gxjevqcnj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/ghylusphg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gfkzeefvn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gotxzfezq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gtmoodlpr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gaahtwrlv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gcnyzduct.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gpkcabosl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gsnvtquhb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gpvctablw.sHtML


<!-- 参考信息 -->