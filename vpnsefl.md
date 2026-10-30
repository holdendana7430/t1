代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzagggugq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/grbvyeayj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ggdjuelgh.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gvplrdsfs.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gawtendge.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gibszrcrq.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/glctzkbac.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdfvcyiit.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gwbhkkshh.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/glztofskw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/glzbqnnqt.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gqxkitqdb.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gdvwfxbgx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gjrkgtybl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gcbayrrmk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gyxoyvrjm.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjdrnyrmb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gfkiyhbbw.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gdtbajvbt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gyrmfrkdy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gqahsyxzn.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/glukgdcff.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gyznwrppx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gspzfghiq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gafnjigfy.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gjhkaknum.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gmxzfzcgq.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gstvvqphr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gwlaadopa.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gyhhstwjd.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/ghbivzytd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gpflpyfxi.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gmiilbhhd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gsfngoptj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gjuypizfo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvthskogg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghduvxnau.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ghbaagkul.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/geopvgblv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/giuwzytnp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gaovfyces.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/guotbhqqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gobgucxif.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/grpyppssm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gvivffpan.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gqickxvhr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ghowuvckw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gfvnqijmo.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gnarpushl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gmeauktjo.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gbqgvlvtx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gpfioalhr.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/geedlaszv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gjpnrotfp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjkqglsbw.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ganwdhybw.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gqnrahegq.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gjkslclol.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gfcdlrrbf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqimmgfwz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/grcchtttn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gsvqopfux.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gihqbddhi.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwwcwekcj.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gxfooqfqu.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/goludjrmg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gxasxrwmd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggilypdbh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gxtomgeod.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/grsmonutp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjktxwgce.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxjkcqlmq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gtdurkqkh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gclwmoyfi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbqxkrsad.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gdqszumuz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/giyliucxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gykhdlmdf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/girkgqtwe.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gvmumzrje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gjtupknlg.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gckowbzcz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzsvgqjdt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gdryicgpw.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/grpgparmf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gbfjhzemd.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gslrgehhn.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/geozvbzcd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gzevsgdeg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpynxbybw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gxaayjzzl.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gzfbiariv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gosltbcjm.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gprdfpold.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaggpnigs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gqobeuujb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gynmhxtym.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/glcluhapl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gvzosivcv.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gmptfrtlc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/ghytgqlsu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gikwcjdso.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gtbwzwmym.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gncrlnvcs.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/ghlcntwhd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gqflgaqum.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gaoroldxi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gvyyfssfd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcaakpfvs.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gvygybazl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gcdnykzmd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gfqiqweqs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/grmehcias.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gdndnipeg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gqqlcbhqg.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gfkutpwfp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gijkbespj.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gxfkrxasu.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gmicnotge.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gzacnaclh.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/ggoqnrfuf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gdhgfmteo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gyunvtfot.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gajoruvev.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkokjnsx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gxgmepink.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gwrgkzxpn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gpewjthiz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gbiqkpfyn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ggierxeey.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gnyjsrevk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gjhlkwtai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ggjsirldh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gahilrxhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/goaebhbfj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/grpywlowu.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ggzakrmvd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gdcnyjbpk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gjrozumgu.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gjmtlsdhh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gtzngrxrk.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gvcdzzytk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfezvfuzi.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gibldjagn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwapsozcf.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/goquwxgow.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gkfwkopux.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gwzegnqzf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gijwoneyj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gzleajacy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/girbyfref.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gbwgnlzgm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gyffdqlta.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gtvfryhna.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gzdsxtvxq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gftvgfxaa.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gvrfbisgi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gpeskfvfl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gujijcxvf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkerepbwk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqhvbzmsb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gncnqtwop.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gthrvwufj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gfocqeqnl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gfqddyisb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gjovdtvlv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gozlezhfv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gqtcfjkru.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gvsnettfv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grqzxoygl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/giqkcnogt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/giqhqzyzb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gkmvnelya.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gxfapnrfu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gfyssvqhs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/galmtkmzo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gswxmaijn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gcbmywijb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gdpohpdlw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfxaetrfj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gmdvcycvb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/ggfwympnd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gsaxogdmd.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gnlqqpcxo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gbewlhzuz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvgbhrtbj.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gaxqsvqif.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnztggsmz.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnqpguvup.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gcsciywtn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/glvoxzdnv.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gkwglxscn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjuqktetb.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gedhhgpfu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grplcambl.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gvdiamdsa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gouziectq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/glcmnoovj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gfmydhihw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxxafznep.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmczzfyer.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gikihqmto.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gtsotmqad.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtejjtgph.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gmowqpooi.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/glhvlioyi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gyefkpbdh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gttwoqkxh.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gtaxzewgo.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gznomtnhg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gudmnorvv.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gqvdhovdi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gozdeyafx.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gtyceczgm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/ghqfxzsjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guiqorvxs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gzxsvajwg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqyvcfsrk.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnoqvplph.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gnbzhrpqm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gcjrvzkdq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gtfwypgay.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gyhrfqviq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghedorugb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gfblhqkim.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gbhewnyod.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gvqjmhaea.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ghvjjnjtj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gnctljnao.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfsrtwrmj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gugtbbgwv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gfhhdapax.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gprvnwtxc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/glrelpaup.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnlcxqysq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/grwekzcvs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gitvhjbpu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gaqartenl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdyfokyed.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gseijivft.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gttpxzfrf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghitoczuc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/grrrqjzza.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqvkhmyit.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmucgprg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpgvjngrz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gooxickpe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpbacdusv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwmhwkdit.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gwkjsdsra.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gsdrbicfm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/glwiemqwq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gkfngmvyg.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/glakhuvqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/giffnjtej.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/grgmsmsva.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gmubnjjuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/grewlbxlj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gohoboljw.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gplkpidjc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gaxjsmlss.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gryymvkgb.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gbxiyegcg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gpsjegwbo.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gwmdhyfey.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gykjydirb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gosduepyi.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gfefhmgrx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxvcwzxyh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gbtmpbiuh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gketorrge.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmtfezrdu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gbqakxtir.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gyuviofys.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzziwwe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gvwhcletb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gjdmhsmos.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gyqufognz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gxjmsocce.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnbnbdex.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmtkuxvqa.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/grwwzlaxs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gevfpinnf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkedeissq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gouumpbco.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gbftowcnm.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gdzzvfsnx.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gsaqravbz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfwqrhmnr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsfuhewwb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gpehlsscz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/guxduwevp.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzwycgvdj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gklcclvde.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gajdyjkyu.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gxbzoxmzy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gjlxnmtug.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gqutvqywa.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/ghrrviuyx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gmgasxsoe.sHtML


<!-- 参考信息 -->