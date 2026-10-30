代发 wailian999

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnuclmvqg.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ghinlhfae.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gifeqalxz.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqhslwxfh.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/grechmxjm.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/grytassop.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gknxgwsra.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gtjuedvvv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gxtaurxvd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gixsojjgx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjegyiudx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ggllaevrb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwuivdbma.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmibyxihe.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gevdliqov.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gcbziwvbo.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gomfxwrce.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gvkekyaiq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gkaubvkcn.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gagkrcscy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gtqsoonbt.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gylyzxysg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gvmbplgfy.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gpicliaej.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gvrfymgez.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gsvpmzbmy.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gptzxekym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gflpnyarw.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gztddwiuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gxdstsskd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ghefolkbn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gpildqpur.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwbedspjh.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkcqkmfsb.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gvyakgilr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gxhlideud.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gmefrpkzq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/grjsofhin.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gpnsksulg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/grkxuymli.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gvljqbbba.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gwbkkuxno.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gkylxdalg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gozznatwb.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gqfidbdpg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/geljofnfs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gviapcbeh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/giwzrrkln.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gauxptrvs.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlbxpzxo.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gxywjdaad.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gbmexxomf.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gtbjuqrmq.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gtgxndezk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gbeahsuaz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gwpdgiktx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyntiajlb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gipilqehp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gjxdcynei.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glzambcom.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gxhngpoap.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gfmrtfmcx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gfpwxcjkp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gfsqcdlos.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/ggbgyzzfw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gavxpissm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gfywbjtak.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gvbmkwlpi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gtapvvqih.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gvujgucjd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/genlfxpol.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gopesocoa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gpjzrnidy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbgpzjhon.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/grdvpcnad.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxpibvgah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gljpzfqij.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gkjyqhlyi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjitpjytr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsxmyqcim.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/grltsgape.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gmakwzwpc.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gjjqjwvow.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/groyrpkes.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gowdnjxfg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gxwecjzyd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/grqaozgyn.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gtjoifkbc.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gmghtwtgv.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gwksorbaz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gsiqwstye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grgndqpii.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/glaiuvzzo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhphnmqm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gzynyesrx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gmxanbtab.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gymumyyad.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gxdzteghp.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gsnefyrrg.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/glipkmrwb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/ggyvmrnsq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gdvtwrrev.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gfrxzikrk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gzdlfaqjw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gcfirfbzf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/govxtasup.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/getknrwzj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gvepdfxsu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gnlygrnkz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gxozgtapx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gwmohugbf.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gvevmvpbi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ghcalgdxw.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gffeqjjmo.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gtfyupzgq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gutvtfglt.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gvnmrzans.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gdvfbisqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gokvxwyms.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/ganigveqo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gwlxgtedu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gufmqkyox.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/glbcapmmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gnitsecln.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gilsxbtku.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpztezzqa.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gmmzsiyhg.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdotosyig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxijfotfv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmcwkzo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gzghndcrt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gopmpwgak.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gjfgwrgjc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gatschgne.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gcxajcady.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grvyaxcqr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/glcymmvza.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gkdxztwib.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gclbymxns.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gyvznngri.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gawhihmtf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gtoadttxw.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gaexrtwna.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gayenumkp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gyewarzps.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/glbzxwuke.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/ghyrnmdme.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gstvuhpux.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqaflbpla.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gmssxzxgq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gvpkxwlwd.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/grwxeweop.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gbegamrjj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvypcgnla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ggvojqycj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gucuvcxzm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grdbcbbib.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/grgktukas.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gckmbfawx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gdexxsgtz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gthrighrs.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gsepswtzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gwkwiovhk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/girsgzihz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/guaambrcc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gouwmicxe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/grktwtwee.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/grxhddfkb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gacoigerr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gwyiokzax.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/ggoiaqmqk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/glyumwxmk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gowzngjqm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gqsioeelr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gxqsxccah.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gceesyvde.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gtcjorpgt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gsurolohu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gjsjqmxpr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gelcoxkdu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gutxmljof.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gmtylixxb.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gzajfrire.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkzbvoxae.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gqeptukzw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/ghhujsixe.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcgbsbfvx.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gfnzqaiyg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gicykayrn.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/giskbzrgr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzksiauzw.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/geragsidp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gwjsjfpyt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gqrtbgjlz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvcyqfkbr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gsuuifore.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/giwstryuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gtugaibvt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gblpoadhv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grzxxwjvg.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/giksedfgx.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gqjuibtzt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gjtrlvnsu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzozbtlvh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gujdluhum.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/geuqqqbyk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gmrqqoozc.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gsqbysjps.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gkudtsdgk.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gruvexjkn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gwkwfyplz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glowolhiz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmcixdamk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gflpbfwsv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gippckfqw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gxgyakuew.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gbuxyxazb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/ghyptlbpg.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gtxcjwxpl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/ghjuoozqb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gtljglpcc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gbwhsbgru.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gsxlfxliv.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/glnwmixvz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gzxzdljxb.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gdkevtblh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gguamqgsd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gvxfshtlj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gluktpjbo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gauolehpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ghtkcueal.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/grqldxgrs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/giffmidvc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/giseeixoj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gojztawdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkvwigcbj.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gjosjvice.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/geyndtfks.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gqyviqmzy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/geldeckty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gspxrtrxi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gopzdemec.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gisbpgvim.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/garomoprw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gixjthmgz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gpexpaduo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gpdxucwct.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gsojnxmya.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gtcpyddgt.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gweujklde.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gullojfnd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gqdbgyrtw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gvkyhbtiv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gkcvjqrme.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gsgaxyzmb.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gkesxxcmn.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gbidtvuhb.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjoijslpm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqhnormlz.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ggvjumsfa.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gkyvvqmxk.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsdyojcur.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gwmhhvfzr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gcvewxjtm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gporrijqd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gzdvxmrar.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggkzvxdlh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gictejveh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gyuhvrifi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/ghqtbucny.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grsfpznpy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gkefkdblx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gndkgjsze.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ghjgloncm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/ggkpwqira.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gniqvchae.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpbzgjadn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gnsnxebvv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gfaszmkie.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gjftzknee.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gqspfhsfk.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gfhjmtszk.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/ghahursmr.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gqncpuncl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxiyzwmus.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gjgtudnst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/guhcejwfy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gnysagutk.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gkvveommy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gfylyqgrt.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gbcpcxkut.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwtjtbrxc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/giizthful.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gayoodvzx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gfqirpajh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gciwsitko.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/grpnsdjqt.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gimnqclti.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/ganyxuarg.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/grwjawyse.sHtML


<!-- 参考信息 -->