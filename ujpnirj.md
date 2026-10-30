代发 wailian999

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/geqgmebzl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gexneikkt.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gdyzcabqa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpuedaz.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gilwvkmzt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gmecraeex.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gdvhjehuy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gvwouctsi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ghdlesxxy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gqgoewfrk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gxtfcqhto.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glwflpyju.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/giqgcnigk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gpjkiqgfh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/glixieeuf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/ggpuekrbx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gfpauwrsv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gymocbbil.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxwyhihzb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gacvljfcd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gatdasiel.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gxcwzbjmj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/ggezvfdpv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gtijyymxn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtlmmcnjw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gybhaaxcw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gbpskbdaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gbwoojdyo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfpjkowzs.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gioewbavf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gtuksbeup.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdcmmkziy.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gaslcsmob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/giwswisdl.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gnlewboel.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gfztsbmtg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gkfcbzjiq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/giwexvhzy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gkgtxkjtt.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gqyztvucn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gntycrrua.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrhrgxe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfrcqnsvf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gkuhrevku.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnlkxrdpm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/glvwmrulq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gsxoaimvm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gedoktvme.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/grlhcuiac.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gmcqmbahz.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/ghrtanjmw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzylrtdna.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gynoxfocr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gdzykppga.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbzcesldp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gwkbaljmh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkwrwelel.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gfygocesz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gxgekkugq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gfiabltoz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gqhrvuuer.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gwdjloukx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gzjjatewb.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gqorbeltp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gvmjkfjiq.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gcccwdamt.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gjzkbhasn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ghqyrtdph.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gjneoeurw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gckuhiyfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gllrfogje.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gxeikjzxi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/grxxrzzbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gwmgsxxrd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gdblaimeo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gknctdmxa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gkuxnzbax.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gvpqabdru.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/ghbjgpddq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gdberfzbn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gpiiolfcc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gzuglukqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/guycchnfk.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gchuojpgm.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gxgpripxt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gymeyflxf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gqmawjlxw.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gwstsbmta.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjfjvvjfv.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gqgifwttl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfiudhobx.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gkasnxxzi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gozklmxni.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gagprgtvf.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gimiktvqn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/grvgpbbhs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxcfdgoji.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ghqfwyrqk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfednwaeb.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ghakikllq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gdxfqlrai.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gztdiephs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gbtozeqmb.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gszqummbg.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gotcrpkyb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmdwqwxfu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gxckqknzb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gzggejznb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gnjpodkpp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gfdjbmjfm.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gnfiriqwq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gireuejrc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gcmimsqnw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gymgpxejv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gbmaivdmk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gycefquju.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gjnsxatse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/guovrbixh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvheybqq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gpjvdkfux.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/girtuqorh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gvjfgmbur.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ghxzjyteu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gtbgehpmo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gpypnxbkr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gguedjewp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gxouonfyw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gkfpxhyvc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gmgyuhtjb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gebzwfskg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gngralogi.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gakmmdsqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gznsiffid.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfkqdbpok.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkjwkdojr.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gifukkqxu.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gbimnrrwg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gvzuswfou.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvihayqsj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvtpyvkqq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goetbjmlf.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gfoqogihz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gufniegnb.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/glvwdavge.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gsqllcjne.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gstoganhq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gmlzvrnwi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/grmubcncs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gkcrfbmse.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gcefviymc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gjaielopt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/grihvqzvq.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gibztbjkn.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gfnohoizn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gyzigcdnb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gezygtrbc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gxshpwcan.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gjbvnwtif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gwewlpzts.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gmxvncorr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/grurlicge.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/guuazkvlz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/geuqhbjho.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjyfhbqkz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gxsfifuql.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxdkbscdy.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gstbabtmo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gymvlojxz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/guacxzxts.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gjlfsymyr.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gqutolykz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/ggzphlhsr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gvrrxmtjl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gygvnnpsc.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpkjclctk.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmfgzgjau.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gigbqfkyt.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gczjbpxto.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gvscpmfpi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gshcmttrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmcnbzova.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/ggvjvnkdr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gpskcsebe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gfmsngyew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gijchnjzl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/giurhlqeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gbsbzvrfk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/grneyrggk.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/ghdghwztj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gctypsjxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gcmdvwrdx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gapfbryja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gymfplpvf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbkishzef.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gfxsdijpg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsgthfjyf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghclzipox.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gcydogskw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gfhtlfslo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwqwblcwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gffocybce.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtjsvngnh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gacimdxjv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gnnvxqsbk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/ghnyjgiuy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gvvvmvgco.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gcbdsxfxl.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/giqztccmz.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/ggtyfcixs.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/geimhnzxh.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzfhhurhh.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/geanvwrqs.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gbavjexek.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/guroolmnh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gqnrgnsvv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gsxzriiae.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gnppvusqr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gcrcuuiuh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gxejkbifq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gjrafcrzx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfqoyajzv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gltktsahh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gyeewxlmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gvgafxylm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gpcvqbzol.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpkguwwsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gjlfxvywq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/goahsowct.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkriqntwo.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gdfdecbrk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnrzgdkin.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gdgtnvvmy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gaklnrpzs.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gdofyqwgg.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gtcwiuxba.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gkvvytwjw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gkxbysgje.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfhgswqby.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gywwfzbpd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/glgknhjue.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gqhbfvaaz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gfmccggih.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/ggrefgkdd.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gojoimshh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gknmqwpqk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gczvseoiy.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gkxuikmcw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gwxvwfsmb.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/guyyldvfo.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/ghrboxfya.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gqdafejor.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmrwfclcz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gwckarmrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gvkdanmfk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gphrnhdfj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gfamtvmoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/ggtmtuwhh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/ghirtqwhn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gyczrmwvq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmhshdqaa.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gccpzgrkp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gsbvhcwnx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gzqjgucki.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gaqibsehm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gxivjfklb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/glnzvsmzq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/golklvnci.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/ghazngzue.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gbkcdotmn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gsnjxbwpb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwsxevomz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/glhsfmaka.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/giorxbykc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gbfhzirut.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/ggiwpcorn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gkzachvus.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gexasffre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gfrjbruih.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gshavitrc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gqqancpgk.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/grvfhwmjq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/govszqqpm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gcogeotwd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gxiusmtzd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gegflxtxm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gdlhliolw.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gjoqnkdoy.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gsrrmoeur.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwelymyrf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ggqoyporx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjhmmvqxa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/goigraipj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gyyzuexfa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gnnscuhyg.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gbjsgcpuu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/grmcvmfaq.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gmtgfzsvj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gjwsrakys.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gkfimuqgr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ggecwogao.sHtML


<!-- 参考信息 -->