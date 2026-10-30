代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gbbxjnpos.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/guzwlblts.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/ghubimxas.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gcjiequdg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gcusokpin.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gccftkzbc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghhixjjhs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gtjomippf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gpxptuaol.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gmdndjjvm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gyvdvgizd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gdvhvqsnb.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/ghbhabnuz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gtzjuzwud.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gakbusoeh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gaszqpshi.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gmgudsstp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gitpyijvy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gfnvfwkda.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/guvgnrdnn.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gjvpukwfp.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gbucouzeg.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gluemyviw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gamyqebgd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gpsjekrwj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gqnvsweuq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gplotabww.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmbqurkiu.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gctrapkfa.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gddemdkce.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gxdwdrbsh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gjwykwtut.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/govakrekp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggvlfphpr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gtgvoaqjm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqmnpfpah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gvfwdgahl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gedyoaorp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gecisbwum.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gmrlcpene.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gxxvvvkeg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/garclalvd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcgchsmdd.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gpyviopez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gzfgpjonb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gwblbzknc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqcrnlfrt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gozqyskrx.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gqxjlrqfh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gftolyxip.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gnyphcxzs.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gfkdordwp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxycdehnl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gteesqzxm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gsmtrniyv.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gpomawlkz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gzvktsdce.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gbtdoiwei.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gddzjyumn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/getulndys.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvjaqnehv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/grwaicuaf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gfipitqbs.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gwqqzdcxk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gyevtohar.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/giejckoge.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gyvvxejvd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gzbixlbqu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzfmxlnyw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gpcncotfz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gsqerprdu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gglbiaaie.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gnkpacvlo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gxepdfcxc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gmewjmyjv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/glmvmwuub.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gofgycazz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/goqefxsrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/grxxunzvz.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gwyzqzogk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gnhudcmug.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gapyegecu.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gqykbxgju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghukevtqy.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gklkvhdcr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gggkwmufr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gpsoviyen.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gukukjcex.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvggrkddu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/guqztusdc.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gsgafcqys.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gglmmnikg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gnnzngwlv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/goloikwcs.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gifxxuipb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gibotdkzm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gbcjlhygf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gdfmpagdc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gquxkliky.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gygjdipeb.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gcdxhwmrg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gnjdkiwfr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/grilutupu.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/ggiyuliuk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gdwaleprm.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfjsnfybj.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gecfmkqim.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/greqwmfdt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gnhrxlnxs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gxtcbijpq.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gagvrkjmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gfgfmrlcx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gftofaocj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gzetfahca.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/ginmbgizc.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gjxqbaeze.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gepdquexh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gdxcwujgk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/galbgnktt.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gisakuzaw.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtjuoaiqp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gurgwsnza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gfabytnwy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gswlwokjc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gcjmxajee.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gitwuuuvm.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gisyxbpmj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gviuqtxyg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gnycadeoc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gkplovvpu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gzxlepckq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/giyjaqqyl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gjbadmggu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gfplpshnd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/golopqqen.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/geutjxnwu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gfuvzevde.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/ganrnrutk.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/giuypowbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gtcwjezti.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/ggihmxvyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/ggvtxwwui.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/ghyzdraui.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gcgnadpoq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gwhtmrwrj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gximdlkkv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gikiqkvyj.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/ghupglwrj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gmawmwkdi.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gtwcfwhqo.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gokdpgtyf.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gchpmebgm.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ggvxillft.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gewvwthba.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/goqovlqgx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gyqfmfpyk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gztfjbecg.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gohbqfkdq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaddkbrvj.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gaykywdjg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gatmljubi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/graoxhtyi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gbhfxhzgh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gtfjsfuep.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gydquicma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gmvyceceu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gnjaooiiy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghidvhksf.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/guwgmuavd.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gcuxzhepy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gojmrajet.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfgbcgmms.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gycwaomia.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gonqjtjuh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gmlhexrzr.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/ghzphvgdm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gomupbdgc.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gunxgzabc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gqbjleoyz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/guvyefalu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfnoxnprq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gdcmiawwv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gntvlpjai.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gbahwasry.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gkwuqchmn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/geasyzght.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/ghmjxqlau.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gbhzzvkul.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gbvrddyks.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gokqeabah.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gjuuswarc.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gttjcskoh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gyuwsomnc.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gzjdauvow.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvqjpqiti.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gcoeiavth.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpcykpgzv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/giucpluzs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfndjfesw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gphcepdqi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhfmnvj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gidnmpcsx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gpbwbegsq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gsuuuiozo.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gjwdeozfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gqlaybclm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gjmoxmdzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdqqkfifz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqsdbubwq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwpkmjswx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gkfaygtwa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxkybeigo.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcsufjulc.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gntppmoll.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/grqcrjhus.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gezynmckh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gxjormgyy.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gwovgpyfa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/ggbcmprsz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gsfgqftog.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/grljobjyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gbuupdpzi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gwyuiauaz.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gjyzyfmfv.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/ggolqsclh.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gwbqrgclu.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/giylumibn.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/guhiknjtg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/giljypkvh.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxtqeqdxa.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gwloqfkcx.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/glhobjffx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gfewglkze.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gmyskdfwi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/getvhcmoo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gksrirddv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxgwcrckh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwonxujav.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gbzklmvor.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/givvvtcvy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gweuamekv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/grjlcebrx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gwwvtdcon.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ggbasjiso.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtziducmq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkigxdaua.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gcxelrvwi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gnudednkg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gesalorgr.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdopzxrgf.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/giwcpkvpf.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gwrdlzlog.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdrtjahgi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gymgyguaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gcuntgyxe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gqbzooibg.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gamfwpked.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gcuzntbrc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gpapnrhkn.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gslraeial.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gjbwykzac.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gheyyzrff.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gyseikidj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gbxoksiev.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/geqfshjhh.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gwitisrwr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gpphbzdbx.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/glcqzwuxk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkzqahnvb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/grsaiktkf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/grfnoxytz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ggauqosui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzxeeedhz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gfrdpbcbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gtysckumj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gemrjvzdr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gghfagyjd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gduupmpfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gblhkpwgl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gepitskxd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gwdkbfsgu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/genfmgnow.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gnoksmnxm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gtmdckefb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghbfigsaj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gekpwhkgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gcomoeqab.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gtivtghej.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbaovihjr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gwecngamr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gcfvtsmfk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gowngfpuq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gmkrgpuid.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gyxrxfncj.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gzpjwjblf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gwntqxkqv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gwwyuecwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gkkwvbzyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gqbnsropk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gesfytwse.sHtML


<!-- 参考信息 -->