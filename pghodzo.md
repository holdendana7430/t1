代发 wailian999

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glbfkabmr.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmjnlofbs.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gugbdggab.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gtilpxxrk.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gmmbvnaxl.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gqcebxznm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gxmgrofdq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gcbsjxrlx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/grsdrzwkh.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gxvrbloib.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gttsbywpw.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gbvgcjoqn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gzbtpmqok.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjcqlegxg.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gnzfovntq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gynadpest.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/ghnimvrxe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/grxxotrhl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gwxzlcoyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gwwppucnu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqnfubunj.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqqftmyzl.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/ghhnlbuzv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gtrdkfgsr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gsomqptat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtdodiskp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gldbvayhp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gqghuxrog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gbdazxxkb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxzflrjjw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gpmbvsezv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gzbpfngxc.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gteusmwcc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gqvrbmdmm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsohhbssz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gnipvsszm.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gvxvyzaao.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbagosmlh.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gjetlpnac.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqwcfkuut.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gnfsyejgi.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gzrcuocjh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/ggaecmqqx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/glhlvmugg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkyniided.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gtrywgzsh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gigggrzuu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwwsxlowd.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gjwrewkgt.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gnillftvr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gxntxanyj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gtcrqhcfb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gkdskdsnv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gkmhrexzi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gptyhowiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gehegmenb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gnduybtvm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gizivgvwj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/galuqxjnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gryzzkcep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/ggqdkvgqh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gxmutkhyn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfijbtam.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/grwuujlrb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfjjfvndw.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gvbafzsfw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/getsgypeg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gulsxvtia.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gwfjwdtqb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gopamscal.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/ghequinap.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gjnbjmonm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbasealct.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gxkpejrzm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gsyoysctn.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gkgttpzfj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/ghfaugbwa.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gmbmcahit.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/guomysbwb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gwwfwzijg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gaosiynju.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gvaihypci.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gbancjfaf.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gnmaevhae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/guihbvcid.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gwdjmddjv.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gokxlqgkv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/goxnmwccc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gioieqiya.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gnzfkidqm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gldivdarv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gigagwjkw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzydxbidd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gizadiqza.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gykjmjnqh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gdxxakdto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gxjucatte.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gappwxkex.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gykjcxlwi.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gnieburqe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gitftxepy.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/glzxmdkfa.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gkfezvulr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqjhppvdl.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gcsnbgkyr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gghmybimw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gozujgkup.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gvqmiivss.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gngazrapz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/goqwnzqjv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gnmwpmfll.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gkwljqdjp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gaoxizgkm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gvmepxtfx.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/giuyorlkp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gfpewwnxd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gbifwdtmj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gavfzrxoh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gbgyoifnz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gdeeowamp.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gruhhryrc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gsembzxug.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gzshyhofx.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gugowkzyd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gmadljyrh.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gwgajmbcm.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gymymjidf.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gzjbsnhpv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzsxblkqw.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gvykvovbb.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/ggwdlidxh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gqxeiypbn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gtivybxdn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gnjicizez.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggjooydrd.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gyvkyxnpr.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gpucsiwss.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gfbtkgawf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gacnxkjpm.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gukrdtrqt.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gqcbhdhgc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gceuafvbi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gsuhiogwh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gpepujlnk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gpoqptixw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/grszdwjkd.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ghdsxwhzq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/glxvzoigj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gctdhbbso.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gmmgllofa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gatasnyfe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gxxdmdkbw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gprfoxvbd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gadhmbaol.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gkaxjmdwf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ghtbilaxo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gxqolrxbu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gcqhlsahf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gspkjixrg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gwypbfzyi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gopfvekas.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gosrgoido.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gkbqsebvq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gnuvnsiaw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/ggqtyrldi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gfhifwqcy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtkoecwzf.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/grrjxktdb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkeerfjje.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gdeqhaeic.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gsapxqrum.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfkzzobuh.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gkgzuvlrt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gwhsnvpfr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwaixmtyv.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gbpwiejrl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grpgecwrt.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gzrsiosor.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyfyveqjj.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gxcgyckcn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gzpivrgom.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gedpntbgd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gtbguldeq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjnbbrfbr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gsyhoyjws.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/ghxtozcty.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gszkchbiu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjdfuhonp.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gglgszmpy.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/grnbvmzke.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gttfiawsv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gqjkhlack.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxfpsdeol.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gdpeirirf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gdwjqbmum.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gpaemjjkx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gmisddjzb.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gdmjolndf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gkowlpzaw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glkfdmtog.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtfxuruev.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gyesgpptn.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gktsedgen.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gfokuolkn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gkrlhkyeq.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gloqncxtm.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gljyqdbnv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gaucyzvkn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/geqqixgly.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/grdekandk.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gchiomvsd.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gokilnral.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/glrlgnkhd.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gybleosef.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwtjsjurx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/ggckcvcgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gymvrnpzt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gskwduteg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggctrofot.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gkxzplfgc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/goccodvxa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gyzffvmhh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gdfxakkcr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gcjljfipj.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gzyexpgzs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gdnvwnlzy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gyxviyodd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcpjdjqxk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gaspahpun.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtwzenmiq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/girpccytj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbodlexpa.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grqwekxoh.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/geelmxflt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gswesvwrk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/ginjwmkwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gutsoamnm.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gdajaogso.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/guavzbhxc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhnqtnrk.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gsahgbxuz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gmvkyqzeq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gpbdtnhrg.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gkuoueoae.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gskdwyiws.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gzertvxte.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gohjvbsii.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/getojpdpe.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/ghsrqsrjr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtfigktrb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/giusygoau.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/guhukqdab.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzqznkeah.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/ghyocpfzb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqclogqdw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gycowkqyd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/grirgnvhs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gvghvwkwn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gqyfmqivh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/grbbrillj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gbolhoknv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfqgvfeiw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gabgtsvir.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsuttjvwv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gymniigzj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/grpygxnyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gpejilocv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/goqnfmasz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gyuwsmzoc.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gohtxivfx.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gimvssnts.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gupaclvrp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gvvjrvdbd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grlzfjuuc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gwhgaiqyf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gsyhuykju.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/guvknxrxk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/givenifvd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/glaangasx.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gwpxspsue.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gkcjzrobg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/giwyfobxp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gcrlxzxlo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gxoqiqpvj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gwcbyvvwj.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gaampozik.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gzibbynqm.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gqkqptdpj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/ggbtxqjuc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftwkesho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gllvqpntr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gmixqrpye.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/grvyegjdb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtpeilqzu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/ghjfzxnsj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmnomloww.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/grdwxqday.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gjtmekvnr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gljpnowtv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gezcyeddb.sHtML


<!-- 参考信息 -->