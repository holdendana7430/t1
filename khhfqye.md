代发 wailian999

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gcvikrale.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gjgbjgnaq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gdgmozvla.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwbvrtjxv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghnrqnpyi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gcliefsye.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/geemhlnma.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkyknsbnx.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gfakgqhoi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/geszgocvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gpegfxvzr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gyztofuqa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gdphabily.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/giokjoxzn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gslfxaipf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gwvtckbtf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gckbdyiuz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/grpjuvneh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gptgcvuvk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gmngvwhdo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gqyetzbjd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gykcovinj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbsgftksw.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gflcnahrz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gxbrgdphk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gfsxnzhvk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghtszltvd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gfyminlru.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gnujehzhx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/grsfnbukw.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gzjeagxlm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gepmetimy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqspaxxjf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/ghewikzir.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gagzxxiyr.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gpllqlacf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gqmxosdcb.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gvtemmswj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gtjmpffmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gcdjnoqjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gytxetoxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gcodewvfa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ggwhuogfs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gnqlfxrui.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcdckeihz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gwyuyyyrj.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gtlxxutxv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxqppnkzn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzaxazkkb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gbbkqnnzy.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gfwlmyqif.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gyestaezt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gfppunxep.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/guhotmmpj.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gfwvcpdlz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gadixgfob.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gjrwzejhd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gnhwjfplc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gulhfowhf.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gsqqdpkay.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/ggaqvfrzx.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gklmgatlo.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gtgmzeltt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gyirbepdb.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gxwmoyieb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gkgmjakdl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gnhvrkxku.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gkfxiovex.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ghaffzixw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gvtzxxczn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gofmvwzlu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gknrwluhl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/ggdmfgwvo.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gaexgcatq.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gkiwmdeqt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvshjpbrk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gzmrqlumc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gnrkgnqmn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gkqdbsnzi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gflucxsoy.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gqjrpcqsl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gwhjozdor.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gozfvrqdf.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gtfziruya.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gcshsolqu.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/goyqnlcvk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdgxwizpp.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gilkjngeq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnemqbkqi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gkohbljol.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggwaxmqge.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gmpleqlza.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvdfnlncb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gjxohrowj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gtznmsoio.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gjchjrynf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gliqhhxal.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gvvukpzmk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gqkmyralo.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/ghkgqxtzm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnqbcxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/govxoaggc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/geqomevdx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gxqjnvagj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqtrkfxzy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gvzdfodxy.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/geocaoeer.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gdoetkfhu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gpwndqdzk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/ghiilgqlf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gwvxjziya.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gjsvitvme.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/glgxvlxxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjaqiaibs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gnrbgtges.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/grzilnrlu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gslsqymmf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gaqbqavag.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/geabmfgjb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gyzttctct.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gmkycolxl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gnhmvskxe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/grfxyssrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwixsborw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gogsfphqv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gzrrsjdbe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/glxekdzmc.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gglxhcayo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gevnmllpl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gqqndtnxi.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjasjozwu.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gjxehjxsc.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gptwhfzpo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gulsfaleh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkvgytjiy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gtvfnsbss.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqghbwisz.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gydxwhkba.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghhindxeb.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/ghszpywbf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gtsmwxdgs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gjbssxjwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gfbpmtcjh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gsrybgtxd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gykxzgcdq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gemvpkiau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gvyyzvrdq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gumzmksxp.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnocspkrw.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ghjvurxnb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghnlvsjkm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ggaxfdqrq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrwavkm.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwbsdmgst.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gfjtczqxv.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gyyjfuihg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gmixyplrt.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/ghbyudbvy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gqjlqqjji.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtvbxvmzy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gciwnmlkc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gjcvrhyur.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ginryjaml.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gmfphdmak.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gqjvrofir.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gnmvyqolv.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gnztawsnb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gmxwpgtbv.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gxrfuhrkc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gmrgnldak.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gtlwbwznv.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ghqicjaob.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gceldbbrj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gicevhdfz.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdwzhxkhl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gtmrbzrrn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gueaquocj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/ghccaenna.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/goemrdsub.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gwkjnouqy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsoxapepg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gwdocivkr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gcexqabhl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/guuakzvfu.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gmhwtwjgp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gtlphlicb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gnluhdcue.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqifeizkd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwwkbblpn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gunquvpwu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gplfugqfv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtjrgzpip.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwafrqpli.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gfadjzpjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gbqbctpiq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwkuvwdlh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gtvkzuopq.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gufztzmda.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gmaqialwd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gftbsetrl.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/grbgludzu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gefgyfeta.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gdqsslovv.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gnoclagpu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gpaucfnlg.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gyardolit.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gukdrdckd.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gtnertrxl.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gsvtlngtx.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gnabzzmhi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gnatfmowt.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gdcpnspwo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ggeismqaj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gktqhfusr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gkslgsqdz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghtikdolo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqmvyxwza.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gumxjykqx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjykbkngh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/giyohenbu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gpawqsyxx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gblvzncsk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gblnfebvu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glxytvgbj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwwmkffch.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gctnbvknb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwixoeker.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ghkgdxwtf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gptjpdxng.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gsohbojbu.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gzftgdnfs.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/grkfzhvnm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzubavjeo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gszihsicv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjceluueg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gtyibxwqq.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gwoxkbduc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/goroohjns.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gytfanagl.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/grxfpfmis.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/ggaojapbv.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gfzjzjhmb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqwaopsui.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gbdyjwvvq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gzsjlqnbi.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gigrmssij.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gxrfyvtgh.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghyozgzfz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gqigeydxm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gdlfismlf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmqjrwtbj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gbmdakdcw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gehtfwlhp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gqypodbsj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gzflokmcp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbxuceiky.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ghrryouat.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gjqsnyuha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gspokdibx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gqajawghj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/godayntxu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ghxhyacqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gaapczhiz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gquwmpjid.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gchwymtcd.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gmvbqhvuk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpgwkeafx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/ggfwopdyj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gdwcfctvf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gdexafqav.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gnymhktaw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gmmiesqew.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gduyadala.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gwodietxi.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/grdeutqtr.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gnmogldpl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/glhfnecfa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gudasumuf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grnlfpgvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gchcahixv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gnfxirqmp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gvgjfzjxz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/galtebjgy.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gllplvbwt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gscwkizjn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/ghelctiho.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gkyfslecg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghccqages.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gytwmasbt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/glicxtgpj.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gqkjqhcor.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gujsbkatk.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gtlruxcza.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gqvtanody.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gjqkgwuhy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gphqnyrjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggbgaxepk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwoabqneu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfplwhfmc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gxvfzpkqn.sHtML


<!-- 参考信息 -->