代发 wailian999

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gaonjmeba.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gbynuvtke.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/ghnlkgqiw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gonwqoggn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ghyvulkiq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glhstfbmh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gfgbijuvh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnsfdhkgc.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gzeangbdj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gnfwphjcj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gesjalzdf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gmstuauwl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/guunidozv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnmnmynr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpoeegbid.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/ghteyybmg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gctukihuf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gamwblkhq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gutvnflaa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmknjepa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gvvwhigxz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gbmufxkcm.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/glbnspmqs.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsgjjtfus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gmvjuiqmg.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gcbxjdqpi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gffyackqh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gtsjonufp.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gclqgpvhw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gzfprnxtb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gwugumhbi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gknovtqip.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gsixzypic.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gihyokbfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gxgbwfcuo.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gazcoeuyt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gkyqhwwnm.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gkygpchpj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gfisvvnee.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gmwplwtrw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gkxptgcik.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gdjiulgwd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gmnuoengi.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/giqnscnbg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gfoiisfic.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/grpedxisw.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/glnkqmonr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gqkdfviyo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlzewtox.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gbixuvhkx.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gbmicsixc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gmtcglyen.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gziqpabjj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gtxxtjmwj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gjnammyzo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gucvmjlvy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gkrlzlqvk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/guepawkgm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gtrxxlpye.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gwsobxeic.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvqnjmsko.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gzwpkjfps.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gaixkztpq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gtmixuchs.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/giptrkgkq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gyzghwtkh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gjlepksbm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gmtngxzmh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqvjzzqcx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/glrrwjjee.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gbbdfqcjc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ggmsiiumf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gtzcmatnz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gzdcnagni.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcjwweyae.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gbbtsgnir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gifizimlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvsknnkcu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/guqkfbzgc.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gujqioqxj.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gujjqtabv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gfglfxuii.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ggwlbmuwn.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gnvqfwksk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gkblyhpno.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gympyesyh.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/guiunxddp.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gotdzuqid.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvqxfhgcm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqyeafzob.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/guphovcxb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gbjugekel.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gnuvqsqzn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gctavkzlt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxdjqfoqx.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/guxsorlft.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gotqkspbd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/guymrxkfg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gqgadthma.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gtahfcxmf.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gbhvdlohz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtojftxbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gufrwshez.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/ggpgqqrnb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gealbidiz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gdxqnfuvy.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ghloajlvp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gzwhbbkiu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gnefnysgj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gdjnhnmmn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gfknpjclj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gqqklritz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gkojcepqh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gegkhrazx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gskzigeeg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gprmhcxas.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjugfvehe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gxfyvpbwq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gecgiztuz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gnbwvudbj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gaqbmziaj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gwmskayen.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gjuckbifr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfteqfrzq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gsbvhvopt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gdkqxwsbg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkxkrpgqt.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gtocpajwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gqaumouht.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gidoztwwj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/guffajwub.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gzhsjcxod.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgsstqlu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/grwyogzcu.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/goxxywbsg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ggzcpjhmq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gujhjivax.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/ggvejiofb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjzktrwmv.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxwocvffy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gomtdabbd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gpniutabn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtrgsgyof.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ggwahoils.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gawghmvsg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ghnttqfdz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gxmnhkcch.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gittsmggd.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gbmrmxdjw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gjbylwcyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gavqvqwyj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghvzccelb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkvqzaypx.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/grzvdsvoc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjelnsthv.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gkyurrasy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gyodbfdib.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gwrogieri.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gysgenaiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbsrfuszk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gloppfnns.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gayhmlvnk.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvrvcgxmx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gckgckrlt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gqdvyffda.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjuqtcdyc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gfgfkvmtq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gcbmbrqod.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gvnuwcsgd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ghvekywhe.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gsaahnipq.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxjafsigu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/glhsqogok.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwdneinds.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqcfgsixb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gnjahanxt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/giyyxyikc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gmzusdtxm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmxkdxxpn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/grfuisbjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gwnwpzxog.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gadngpejo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gqokdcnho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gcfneqzgg.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ghecreamw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gaziilukd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gtaelvqvk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gduepfmah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxnxtpktw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjahtgecg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyptxffns.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzmcowthm.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfstulgvp.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gdidnqqup.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gevdfmedi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gzonsibwa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/ggwhsiibk.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gsvtrabhp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gfnuebhik.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gveiakidh.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gcjeiglgr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gnogzpvcf.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/glpbowbon.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/goeqqjdac.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gmpqrmbfl.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gscrquqfh.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/guscpujus.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/grzovowja.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gowifbgxm.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/glzmcuipw.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gxlcjlkty.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gpgzvjfzm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gpluecshd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gaqhbsdhi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggqufxwec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gnmhmwkdx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gzlkvnolu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gwujixxwh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gfhlhkaba.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gbbdlacne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gzytbveba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcxengtub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gnshowzab.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gxvxzptea.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gbiafhcsj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/griewfull.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gmjamtuxg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gzofwxlah.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gptigqbvq.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gpmhpaofg.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gpyllgilr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gpvisfjwk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grkxfkpjb.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gusbwamhx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/grgxqrfay.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gglwyeotg.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/ggzlyeolw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gqcuuvgbd.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/glfskowcc.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glnvbbgin.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gmowqxlau.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gkmbyjupw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gpmdavtdd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/grcromwdk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gikajoufy.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtzucvdaj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gfzqtbwuc.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gsamguofo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gkykxttja.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gtvtjgozf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqkgnnwyk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfxgiqidc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gggqngnzh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpkeuueuw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gkhhbmpiz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/glinxizsa.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gwyxlvrbj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gnmzzdlwe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtasfwkly.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gzukydbzv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gpqfhwbxg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gvztmjwup.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gxuvgramu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmxcamuj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/ghdwzbqvr.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gydrdaadb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gsxwjrvbd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggfwsdamr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gwphnbrxw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/ggzwmapbz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gtnqgoycz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gkuiqgqpn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gzgnbrcze.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gqtivkgqt.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/giesuhsyf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gojwceowg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gytmrezef.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gqacnvosv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grtkvrmbc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/grlhlcipk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gnzdqaoru.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/goyrafegc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ghiipbkvl.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gepsxeccs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gehatoiys.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/giigzglvk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/giaratlva.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gifkxvbsn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gxcqgyxtb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gaolnmftv.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/getnlkvcd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gwtgvayew.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/glxfsijbs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/glprzsldt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gakiwpkcl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gsganmpuz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdserzejd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ghbiewnbi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyaictflq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gprgqwrdy.sHtML


<!-- 参考信息 -->