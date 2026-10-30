代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gtomtuylh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gmzcwzndu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gaqumwetj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gfwlhfeta.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gvxfvnyzx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdjthdiac.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gpqihggec.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gpmzbxlma.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gjlkmyvxx.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/glbimxkkj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gemcxjmun.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gjehsnfcg.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gtgqxkdkh.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gymwrvqzr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/glpanhtjb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gyoxahhjg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gddwmwtie.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/guxfjfhyn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gsfhupvzz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjdvzjski.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gbhjahmjx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gfnettttz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gdyzoxufo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gzshtwlqp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gmmypfehv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxdlwahdh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gfycxhuzi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkfzksars.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gtfzvqygs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gvrpxjxvc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gtxtsetim.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/ggnbfvrxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gzxqkxffs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gfoaoxuby.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gncinwltz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gevivuhji.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkqkhyndd.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ggtpaqhtm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gifshasbr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghzkbehpj.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gnervttmf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gytywhiuv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggxfzfhet.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtnyjvymd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gwmmoiebk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/ghcjopbrq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gqlkuflfb.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gwrrpzypj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gokzzwqma.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/guilkcnyy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gduffjqug.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gtkruqveh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/glvenxyoo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnownlrrm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gmotifheh.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/ggpgpoqrk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gqesexvam.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/guhqazdfu.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gyswoyeuj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqnbmephb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghhfdlooz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gunhepnns.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gkshptmyd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gibcwkyhg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gksrfelck.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gltrlaobv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gssihqpwh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gjjxcvbft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gpqplkdvi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuomftr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gadgndcyv.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gdfcipvsp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gkvluhbwj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gfhgyfmld.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/ggxwfgvsr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gwfjlggbk.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gnckdzjnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/getwzvxqf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gbozwwiug.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gjrbpyqke.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gkcvwuewy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gdeqrgotb.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gjxrhqlgy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gasjhigep.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gubnjjjzr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gssbszyra.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geitqgcut.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmliabvga.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ggnywilxp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gmyfywfyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gzpbkzpkw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gakpovyrl.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gloiovbhb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gdiezacak.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gsrozkpmb.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gheucaihh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gvwqaklju.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbzfdckda.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpwspruqt.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gdezfzeuv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmevgugdk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gqamhsafl.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gdqyfrmhr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gqdcifohg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gkyanengd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/grecrsrdu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwdwuexs.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gvfzfcgjr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtclucukj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/ggtxocwmk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gasbtxpgk.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/ghdlmswnd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/ggyyzunle.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnivvoqho.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/glnucqlfg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gufejzgpc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gulvbvjdq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gsfrfwcxm.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/giqvvwtgv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gakoeayiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/ghdyjulxg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/grbztsiyk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/geabqlttm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gqrtcgxrx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gczhiexbm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkhxrfgom.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/ggflyingu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/ghbetwgvq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/grxyecbwi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gviwwzdil.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/ghvutkuen.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gwqdjlbph.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gmfavuzby.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gqlinjcgh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gexwcwofg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/glbaitryu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/giyyxjjzm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gzzkaqewt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gooavgbzw.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtjqmfkwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gainvakiw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gjfdzsgve.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzjntiffi.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/galnyfgij.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/glthinyeq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gutdaokhs.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnibamvlj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gaqkegves.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbbovaohq.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gudaypygq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glwrpskbw.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/grqhjowsr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gdqbgoegq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gakuupkww.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gxkfeprlj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ggnzytlfz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdubelijw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gpchtewzk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/grzasrkff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghhultsrz.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gylgadxrh.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gohsgdkkk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gvnibuotn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbrtmqusp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbudkrhzh.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzdnmzjxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gyfxrtuhx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gwfizzzfk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gcxtuaemr.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gokxwxedt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gmrwtnvzn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmbxdbjxv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gclldxkhk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/guhqfxmrt.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gzwzljsno.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/ghzzkdbhq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gknxaaejy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gsldjgfiu.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/ghzisombx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gwphvhvlh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gnhcldcwa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gmjyaetii.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gtjfjwvhl.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/giajxlpjk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gnilkgjrn.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gzlczioty.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gegklmoqk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gcxjusbij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggpsnqcca.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gcxtkorvn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gudbuuoti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gldxshhtj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzdhjynmd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/guejtgzts.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gaxvzqzwy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gjfeivowg.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gljyxuxzh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gdaxcaief.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gwspflarx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnpaawzew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbeadhqpe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwawmecez.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gccyqwhoh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxbdkhjje.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guqpkrtlj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gezxysuno.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gfajiwfqd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/golvaodjt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gwohtmgex.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/goxemofqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gjpipypfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gzzekycmr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gjwmnwdvk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/guwgnaeuz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gjulustcx.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gifomamuz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gsvtychuy.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/glvugpmvq.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glmjdrwvd.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gapgpgpfq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gxaxdlmyp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gevseshqg.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gxgmtomen.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gvnhyvkfe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gceptwlqj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxkvfcgpw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ghxmdhjos.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gquiaatng.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gxnypbpwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gyhxwmdjs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gonxwqtae.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gljbrughq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gthfqioyz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gkowdejwm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gopljbjxk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/geaeaubms.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggdniufst.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghmmrdbsd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gawuqtbrh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxfxxwwal.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/ghuppxiby.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghmglygee.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gtzyvdpks.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/garnsvlwp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/glwyeewzv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gryqdcuks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gutdvnqbs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gwvtcsows.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gotbcjhso.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gczjxqkfv.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gfgrmusoc.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzdsoottk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gmmqegwya.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gyodlglbj.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/ggoyyecmg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/goszqhcwo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gxgqdtoxy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gikwvywzw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gcaomnepa.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gexuowdjq.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gurjaazdu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ghuwnyuxb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkxqtgrus.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gkseskefk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gjboivhsv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gdivqopjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gswryjvcu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcmwqbkdb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gusyxchzu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gacrujkag.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/guqjkwjud.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gyoktixhb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gbxhlxqkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gjhhrqydl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gklyjtvhy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gxsyebasy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghsqqbdbh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gpmodosft.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gtjedtnek.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gjnkahrdq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/grvzfhtze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/ggmbbwkoy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gzylchepk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gultnghsi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gjhwipwdi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gvrvspmxb.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gyyeqrlwm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gkyrakwaf.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gyqucmmxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gfuihuakx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ghcslypik.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvvljcqmj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gwpmvnvfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyjjqvfzr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gyixqnpga.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gedqbuqqi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gjqxjuhhe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gnjbaycdj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gqwpitoaj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gfvbkojgz.sHtML


<!-- 参考信息 -->