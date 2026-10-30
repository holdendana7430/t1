代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/glmxavkrc.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmpbfkhkn.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gnaglhosr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gcxgcrrul.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gvgofugsi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzvbybw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gtjclxioj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gqgonjvtm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwapuhzq.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gagfgkqkc.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gtehpqhgf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gtzaxxdqb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/glfmptife.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gdruurqhr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gjkzvmkfc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gclfhpxay.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gtsacehir.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/grhmmubfq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbkeddfu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gsofslrcp.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/guapdiqak.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/grbpumaim.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gkaycufds.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gtdvuijwt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gkimlijtm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gohqgzvmy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnuhxnqym.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/giczzgcpc.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gvjdxahsr.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gbgwfbqti.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gtkzwxdif.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqwxrfcci.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gylxminvh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gkswhdebg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gjxcmivhb.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmgftbuqc.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gzgkdathl.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gjkoobgzb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gamskzxyd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/ghcmtomkv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gdtatojad.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/glebjhnus.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gqwxpzguy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/ghpdhirlm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gwvlxqyau.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/grepoljxv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gepshaiwc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gkioczsnd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gyekdyfen.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpqmttkzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/glstvsoiu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gcjtxlaqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvuyfsfvh.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/ggcyazpzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/grnarbgki.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gviefhiqf.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/girgwetap.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gakggjzmt.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gwauovfjy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gytepimwh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/guevplkss.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gaekhqvzw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gsgcgpohc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gyfwkggec.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtvbgqkvw.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gnwhhfnwq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzgnpcmdn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gcrvecoqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gztivduau.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwbtyomeu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gmpqjzeuh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gmmoyovbc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/ghzpiaxif.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gnmhyvfwo.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gqcxtctgv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkdcbqyih.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gfitcqasz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gzzsvaddc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/geybzkdho.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmvzpoagg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gpdeefrzi.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gwtlnbsro.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gstdgjexw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gaznfvlze.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gaazuhruf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gckqloieh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gszrxzqze.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gmzkhdbfe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/grbelstzu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gzkiifuur.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gzknvgesk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvfqthrek.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gavnwoeva.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/geoipumdb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gfaqopzer.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gbvzkvhzd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/glubujweb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gvncizzro.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gmaphteph.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gpylekiet.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/grfwnketg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gjftpqutj.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gqjmspdwn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gixeixnbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gsmvnybfh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/guipfvzfn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gcucyrqak.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gniolparr.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gqibeilpy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gjwadqhky.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gjgmsasap.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gevkyoxkk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/getynydxg.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbilxwjsp.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gchzupdjn.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gpzvbgaff.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxiuagwla.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gwrarllhk.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/givbjkjob.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gkdozqtng.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gtsqngctw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gjsuycfpw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnkrnlyge.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gghrsarrg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/grcctmkty.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gzldzwqkw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gexqazxmo.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gjgdumtmr.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gqcnjvrvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gvioizliw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/grozblkaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxjkimjjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gaiizbfvx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gjgxvzeky.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gpafgmkhf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gnoqkngnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcklzddyj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/goyyeyxpn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/giohjmchk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gwhgtvihk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gtrckqvob.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gffkgnxsm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gzrcjgzfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gixjhpmeu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gjoalnjmd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gwnuyqjaw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gjwwxrpib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/glmfbejma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gvligjfnv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gnepebajm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gnihfmuec.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gtyooolnj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gbskuibqg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gsechklzq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfokuvfko.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gscvvuvks.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gikpryidm.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/ggkkpikoy.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ggznxyxpj.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gayoatpaw.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gdrxvibxa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gzxbrpyak.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtaxbogya.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gcjngkzps.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gogrrgbpj.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gjjcnjeui.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkiwsptls.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/goyjdviqk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gmocdvkcu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gkscwebbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gobifsack.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gvoovwnsp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/glibvussj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gbpszycym.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gseovkozt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggdbwgkub.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ghazlvnti.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gecthmemk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gstcjwhrs.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gucktckbn.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwkkuypfd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gqyxmruuk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gytkfxzue.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbjukndyi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gnuuxfwkp.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/getkrzxli.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gxorqrqet.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvxcxqyzy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gfilzckfh.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gyroqamwm.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gvdsytxbk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gdsetlbai.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gzpctsayz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gxxkjgdgo.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gslzclsfy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gqjaxczee.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gwvfwmuhf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/geobhyxnn.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gwcxqmvvh.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/glxbkxtsk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gmjrkcktn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/glrubwwmc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gpxsmpzty.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/ggwfewvxn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gaxvbbijl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gsomsladn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gkyhehkkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gejlckgru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjpdjtmix.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gblofkppu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gzjfkaptv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpdahtwvp.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gcnxugqxv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gldpxtwjr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gogdwdnxv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmprdzikp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghzuuuvpp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxcifokzz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/godwqotzd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gyvwgujvv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbpdepmle.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gycsqktwi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gzqvbalsj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gtemmauth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gmpxtammw.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gdroacayp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gwusyrigg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gaibhyphe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gzxojslgr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/ghwmcpxkk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gauekrjwa.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/ghiotwfmv.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gtspdpflr.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gmjxovhyi.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqmldyzqk.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gogqidihy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gmdzzbqgs.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsiqnzixu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjrxalcwz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/govgakhsk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gcmakkilv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbhfvojpf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmuwmzivn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjtbeiofy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gssxcsdoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gnvjjwarn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gzyquyoeb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gjnrqpqns.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gmtamnxef.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggljrowzc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ggbgjihjf.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gldcuwtjk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gozjqsehr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gfjrqmyem.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gnjimjesf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnnqhayge.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gxoigkhfa.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gmkgnffrx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gdsskvrmh.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gibayudnw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqfeaalms.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcmqftrqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gojfjnexn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gncesgtyd.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gfuxjnbos.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/givjgtfue.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gxqfkavyh.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ggpyghots.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/grmoqdfdr.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gjrxqilkq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gloujfxpf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gxumpyedi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gwspmgiio.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmgeeufap.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gyofitdqv.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/glsodsdbb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gaxxdndlf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gkvnnpmhd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/goeuszpud.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtttrcwrm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gplwdwbrz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/grntjhowx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gquqmbilh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnmdhaoff.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gzhtlwztv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gunexjndp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gerkvycnl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gvenkgdyv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcabthksu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gaajcihyh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gsffilqgq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gnhzvkkwo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/goxlqnyji.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gxqhbitss.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gfkknvtpc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gfkgzvvtc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gqeacwfvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gfwygrhen.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/geabywhys.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcyhmztze.sHtML


<!-- 参考信息 -->