代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gaxoigevu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gcyfdempc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gfdjjidhb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghsvlemjx.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gcpamkgvf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gsjlorpjl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gyrcrdxuh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvncbhq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gdfqpngxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmdfvxblp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gpjnxdfuq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/ggbcguyrj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gwwvrrrbs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gfmybjmtx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gsyuqcfzr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gccjbwdop.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gemwolefp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gxoleegvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gwqzbzblk.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gksbwhusj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gjntlnqyk.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gbaqhtzur.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gegbhyypg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gvottsvop.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/grhmdqcbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gmtfzeccj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gcgevotga.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gyvtvbrdu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfepwfdpi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/grzavyfsx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gfkgyajyz.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gfzwfycsf.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gxiscxhjf.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gyrzygdyg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghulsmejh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gaaolknla.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/goolnvwry.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/ghogisavn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gdxvznzls.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gihwwxdoi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gtzdjupzd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gdzjitnsc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/geudbkson.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gcemiyywr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjrnoihmc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gvejdnvda.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gxtkskqmw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/geuipcewk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjohjohuz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gmxrljcga.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gqykolytv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gxsnyhqua.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gbameaaez.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gmetcundf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gkpuobcyf.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gdxptbfws.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gpebprttq.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gyuknipbl.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gvirbascc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gatzempvb.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gativhwyg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gosvyaxop.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/ggmwckiix.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gvmliupqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ghqqegitx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gvfflawor.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gfuxtbyoh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/ginowvagl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/giuqoimly.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gwdrxvbdr.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gotwnzleh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gufyizuga.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gcraqnzsn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/girmkcpoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gsjywjtvv.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gvxijsihc.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gtoozdfuk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gpyimuewl.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ghtfvezbp.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gianinfqa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gpucdtllk.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gzcgdlmpc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggeurxtxy.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwklykvyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbxskto.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gaipcxoor.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glczrbote.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gjkiuenjv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/glbznqewt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/grhslxady.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gydhsqmbi.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/givqipzpb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/geoyrprst.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbwlxqzvi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/ghftbuyab.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/guueysryb.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/ghsviiwqu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gvxbzxoxb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gyvjjwsbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gyodoslnh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gsnlbwgvz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gsnqjvncg.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gptmzvesw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/glifgyisi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gfivgfvol.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gjpbphycu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmxrlcnaq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gikphlmmd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gfhzlxabl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzdwnlvdz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gbxhlgpih.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gaxpjtfcn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/guxgawktd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/grjfbfhtc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gkrshwaow.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gmnpirhhl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gdlpuzqdx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gueyntvka.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gczqcbcwu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/glvzqxpuf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/glbtbbuok.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gokrjzlhw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gaplroiqr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gycwnmngf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gtbtdpdfw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gvqpnqamv.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/govsxldsm.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjvulwito.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/grtjmajxn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gpsqclfce.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/geuursebq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gugerzipj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvnpspfnz.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gngkrnrdj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guuzdruln.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gwfdhgehf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gbamsnyjr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gzffdevcu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gytfdvcvv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gadphcigq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gmqhieyuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gtnkhztxs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gmcnqpmdh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gponjouwo.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gdvrhunke.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/ggjpjqxyh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/garuforog.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gxkgfccxj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvmplyete.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcektpetn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/goepefagn.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gkvfrtlwh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/giflqmfrs.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gyentqdfh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gsuznwlii.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gpfoeanqv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gatknssti.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gxknhavmo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbkehglvc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gyhnbkbsd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gvogxqdtg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gbvfnvkbj.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gwbqscxiw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkxpvzx.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gequeoiog.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/goxgegkjq.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/grqdczenl.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gqrqztnia.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gkbxzpxjc.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkbvwhyjx.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmodhovly.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gyzodelye.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyuiosvqm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gnnfhanbr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gppvpgxjw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gboutekqv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbdwjifn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gccdbtfry.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gfqibsoil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gymkwgahg.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gihcivwbz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gfoelhxam.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gjvmaailm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsqzulius.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gslahmgsq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwdlvprob.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gggojchbk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxqqvtpii.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gppkeyzwg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gejplaqpd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gxrfojjzo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtjraljwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gfokcythp.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gglokfgjg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/googfmmyy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gypnnsmrg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gnsexzmpj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gcfjjfbrs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gssrwuznm.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gkxkziqka.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gjbfprjwz.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ggqwftktu.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmmaoehrg.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gpfhcnfng.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gdzivdfdv.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gekekczhv.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gfxfnwtrb.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gcbjxwwbw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/glkrdhfqm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gmmltyagu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grrtheulj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gqctbrfpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdpyipatq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtqxnbzg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gliyyfzar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gphkhpuaf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gzrgayqxo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/glwsefbhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gsofkukxb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnldgxkdx.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxbewqjdx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gtotdqsla.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ggdbbmupi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxhlbecfu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/grnsraryb.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gvofyzlto.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/grpindcvw.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gdjltbpyn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/goepmqach.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcizasskg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gomvzwhhc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/guwdvgfnw.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gaiaidttm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gqzqhxgio.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gidzrfnjs.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gjkvjnltq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gtihuiikp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/grmigucnm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gyfiluauw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/goohdklfh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gfptfkxpy.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gkvfkoran.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gtpsitkbl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyuajnahu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/ggosjdtdy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/geyfcwzty.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpycmksnx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gofdiplpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gblvzzsax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gqkdeslvh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gflnibzxa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxydvbeu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gbbmmbilg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gvmkbelvp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gxnfgvpjl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrcclubd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gqmqfkkag.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gxcsopnhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gsbfeinik.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gadwchkep.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/getkexeyn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gmazrrnyb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gsjftdbbl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnbgfhyku.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/grhykspqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/giawmiocj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gcrkgcuva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyzjckjei.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gskrgestj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/goytpkoyl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gekvhhpgf.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gdeifqgys.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gbcmajehb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gfirbuzye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gkmrrsbhj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gypwxrbwv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gmcsphied.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/ggkkijdlw.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gsbbwitfx.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gbtpxgmgx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/ggnwoxozj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/glvobnfpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gzisxeppn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/giqazramo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gevafiqcb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqywqognt.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gpwfarsed.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gxwapetwq.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gogkatobo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqyrzvclx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gjzuvxrjh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gduiymykv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqayvxcui.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gzvuwjidr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/goodowcic.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghgozdymx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gieozqpua.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gccexzokx.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gdqlitjmk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gigqbvvzs.sHtML


<!-- 参考信息 -->