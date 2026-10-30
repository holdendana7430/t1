代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcramzfwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gcfjfevpc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gggthvbrv.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gvuowoicf.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gavnbwiuv.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/giwazabfd.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gsfwrebhr.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghelgikqs.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/giicgacrm.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmbmfwcfn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gmhjvenuz.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gsgirjfvz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gvkxclgcc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gfnaegmkj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/glucbrjri.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/grevctyiv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnbinmquu.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gyeexkbbr.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gfjtjliwy.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gazcjexhx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtewjbyzo.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ghvbvpung.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/glcajbafn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gjuztdgon.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gldifhcqt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhqnzhi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/giaanqneg.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gtrchpkhf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnfgumzsu.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzsofulwf.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gmihfawid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gdrhgrkoc.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnkytgjpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gqzdlbdjh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gkaxevgxi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gvrclxzxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gmbavwbxw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ghjtijvch.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/grkgjgrpn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gqigoqvim.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gbhtxooff.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gghsftxxf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/geeyisoav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/geweaylip.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gbtigmesk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gvuwjarzt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gfiapsbpv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gyiuimayn.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gauvhhnyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gikvstbbm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gykqpkood.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gopymkpnj.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gmqksjsyj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gejfqjvez.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gjemkfrdb.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gzavilnur.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gbaotgoeo.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gjefxtphu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/guvhbyydj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/grmlrcpwt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsuvzfrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gdxfolovw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gakyomjru.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsjsbzach.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gtvvvipwy.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gvcbzhuro.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gdtecgzhv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gggkswoux.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gvanvbcwe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gspvijntw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gcuoohzhx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/grhocolzg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/grywvpmbz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gcgcqamuz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyltwvalk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gzhptrokd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gxzjgbsws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjwbholgc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gaixxlsks.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzgqkghri.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gqbzobupx.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gdendaqjk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjujrsumu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gpxcuhrdn.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gbyrqeshy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gymtakdoj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/goxaheshg.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/grsuyzizg.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ghmzbprpv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gauswwgxq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gcecplfxw.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gepbpsdsq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gvvakbkmm.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gseyyssmg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gkakqczjt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvbqfgmhk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gaoavgmac.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gkfwgueqs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gdirpvora.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gkgihxgjs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gjyuhehrk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gbwtumvar.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gdnhgjeob.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gxzatmtsm.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/grazphlvt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gknodrazu.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gsmishzwd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpahsipld.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqvikgtkk.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/grchazbsh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gmnryfqdk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gotidvnid.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gsoeybipb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/ggmcfxzkg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gwydbkpdz.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ghfcwsehz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gdecwzkwc.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gxetqnufb.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/guytltxzi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gnxzufjmw.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gpgpybqop.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ghwpwbkwl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gwwypptuk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/grcnionqe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gpvtuuoiu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gujjohkgj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gmppqeqwg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gbnnspmya.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/ghbeptbyq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gwcoqkooy.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gaiespula.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gsfzldmhp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gffevurke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ggfhnuclh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gnzrwxruo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/giocmuxlk.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gppchkgjs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gkzwucopq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gapkadvlc.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gofbzyfgx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/glgvkcjpj.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gzbhsgxza.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gbalyfzuo.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gtevuybuj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkjgxwnwf.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gephjxicj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gmryalpii.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gkhsqoqbg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdjruoyuu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgknjli.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gfhpoedwh.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/ggfuasaxt.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpyrmgda.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gmvmzapot.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gwkxouszf.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gimorzunr.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gakfwfyaa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gaikxuxll.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gsegyujwe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/grjokmmsh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ggvetwulc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/ggzdlhvzf.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gsngfchvy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gakzagugi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gjkdppirg.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gqgbcwkmc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/ghsmukibd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gvhximgyw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gxpzohkfb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gutxwkloo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgawifk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gsjeckuiv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gtmupnpla.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gyijfggeb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gwgawdpbi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gicjpibmt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/grmsztcyz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gusnvulsd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/ghnwhrzik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gnipmyzmq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gvcofstdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gqmpsrtce.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/ghagyobwp.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/glhjcfqpv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggqiogqtk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gabnaaqss.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gynizmfqr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gusyulrvt.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gxpitmygc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/goxoyiidl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gzsturhea.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gxgwyxcqe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnpilftul.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gtkekfxxx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqrudntco.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwmuhhfix.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/ghrpicmkn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gwugamjys.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gvvyqkkqt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ggxfkmowh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gjwjpnama.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gyncwgnqa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/geuwhqfft.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkmejnrzq.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gnvdiuzgk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/glpaholik.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gilcvvoda.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtmawmfpj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmjqxctgx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gktbrhoaj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gacyziaqh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggnaqojvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gliaacvew.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gdehzpfzb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gtaxralnz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gazktcrli.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ggdgxylig.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gnwkwhnmr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdjqhdbqe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gdxgfbfkp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gnfnijkyb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gpeiuemuj.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gomurafrx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gbdtrxafb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/grnagktyy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gybvakgqg.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gngemmmbw.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gvimsxehe.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gtvhelpew.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfuukmtsi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/geapfyxlh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gczalutgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/ghzlooaum.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbonrruzk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gcjmfpsjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gnnyddpje.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/ggzcrnvoj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gsadkbbvv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gsjkvpflf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gficqdbfu.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/glfbqryim.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gptogarey.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gcjgqyfve.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtpytfizd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghyqqcxyr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxnusmkqh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ggjjbekmu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gklmvnygi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsxuykdxm.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gktbcxqou.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/ghwxooutq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gryctdleg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/ggglmxtir.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gvvfbuesd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gwrfvfazo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggffzyfed.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gkzjdnmxq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/ghrrhnewp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gxnccvvsn.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gvuextnrh.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gbteqxkzq.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjaacilfv.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gbitnyvfj.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gomxqkwis.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gsatambhr.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gidpunlbr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gibeoqhfw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gcizopdoj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gpggagrsq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/grjnrjkrp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxssqgpll.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgxihrx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ggfbxagcg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gxvowmgws.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gvzxbwham.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxwpxgexb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gbqnqfrkw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsphpgulo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gdfkbuuhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gelcmizmr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/giokuoruj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggzqgqddi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gkiyrrgab.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gzqsonips.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gutyyotdw.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/glrajiduo.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gdktgdtdn.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gyluygiik.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gzvaxdoxs.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzmfrgszd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gldqjvsmv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/glilwbrtg.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gnvxxpakh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gpqxvjhfw.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gajfmowwy.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/guaelrzgd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/goapmiifd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gnwggquto.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gskduqtji.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gchztbxoj.sHtML


<!-- 参考信息 -->