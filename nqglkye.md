代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gzqktqefo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gskmiobco.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gojkmdbgr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gpppszepr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwfihirhx.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ghkzzbpks.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxtasptmj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gqqoixbli.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gqvgnocjl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gxhmkuvoi.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/goioqjhyy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/glvwlwbce.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gqjljeubc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gtiqlpota.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gpnitviiz.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/ghkmyyoko.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gjulbtnng.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gimnpgifh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/geexzsmjt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gmsmtklmi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzeifdtgh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gyhyeznem.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/ggstxbsqx.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gzyshjwrl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gjelbkxno.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gkpvdijoy.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gncxzmorz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gagozlwda.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gbiuvxrry.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gponmvshv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/ghmylnwja.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gkwmoqond.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gezgcruvq.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/grecgrchg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gjictkgsb.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gapdlojue.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/ghzskmfhr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gwfokboco.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gesbwneds.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gbjinppgl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzutjht.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gqeefbzct.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/goxhqgnge.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gojexhlni.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gtyzhsbta.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gaznmsklr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gllgygqsz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gnewvmfbm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/guzlrkaxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gsdfsionz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gxpyhfvak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gudsmqsed.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gmosxudij.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gzaxhrmqy.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gejipfbgu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/goqyaczrj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/guarivvkd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gxtnnxjyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gbpcycwcx.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gdrwwuawu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gpaatwkkx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gzeglvcgo.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gwhztbksc.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gujyqcfza.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gkuqualqw.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfslelsdp.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gbnfawdgu.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzknumoyt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/geslmuwkx.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gqsjgrdxm.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpiuirsqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ghnvsbocb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnsdihxcf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gffcyoppn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gerjnmgdc.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gcckfgpkq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbcauwmnh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gwanwykhz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/geojjxzwv.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gjxhgbadf.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gvwxesfqb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gbajrmfye.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gwvmprrsh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gicqkfjrg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gmtrkgnfe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/ghkekbpoq.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gybnadjpj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gtmpkrvwn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gilzieuzg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gjhjzalyv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gcpguskei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gitrhzghr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gbzznwtnl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghestixzi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gpdvjilla.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gyzqgqwrr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gqrudhhqr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gaobqogew.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gxqgzstrj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gnuldqicz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gtpodusvn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gasoazami.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/goihbuych.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gsgryylbw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gjufirjag.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggzoqxcjc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/ghkdzgxez.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gvcccyeta.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gzvslloyg.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gjtpztquw.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gumospiob.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdnuvhmfr.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gtokjaqtx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gqqbaroyi.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gapwwxuaj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gqkupcfyx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkgdfenxj.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gunfhkurk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnakqxzpr.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gefuclvtz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gfmqktteb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gtvmzduki.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gobpjnxgx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/grbrruogi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/guuqmylxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gjuxovzka.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gxqdskeiy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gueiapesi.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gbpyhstpu.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gmvskbyyq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjshwopkt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvivcaknk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gthoeremu.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gjpozlhfg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gduuzviar.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gunckjhtp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/glvhyvirr.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxgyprosb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gxzdvahfv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkdvskdzw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gjirrsiuj.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ghakpkyzo.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/glqsangqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gqnrtmwqn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gzrrjbdls.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/giugnxjoh.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gsfdskcvq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gcpxjbnkw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gqduixifc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gtcatjjwc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gawwbvboa.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gaogisezj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/ggobjpmtd.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gsgplymcs.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gseygxovk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gfqkfjrgw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gsdjnptsq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gxcekrhma.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gunmdzfwq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gydzvilum.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gbdstkovh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gvuvfaier.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gdepuxyjg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpxznpfgy.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gyubmmpmh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gxdfxxbjg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gbnbhifag.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkqydevig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grfmebggp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gliibsksi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmwhsnurp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grzecdvww.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzfixrhat.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gbvdadgtk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gsfkhtsgt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/giwirhixo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gvsqhfdyy.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gkzcamjsl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gwqpulfgo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gcpqhtxqq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gasvsxxvn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/grlzcvnwa.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gafkpvnml.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gdpowronu.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gknpmhgnx.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gozljgomq.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gnbehsvfv.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gkxwzexpc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gibhhmudn.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkszdvjtk.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/grddtphoj.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gkeqrhrrh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gnxdrtyae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/geizhjrby.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gwhmbzxuy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/geaadsvqp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/geftvyehf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjldgujoz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gonlrioul.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gheurshja.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gqtmmyfxg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkjvotcwq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gdfphnhoh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjahxvnrk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsalljkfl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gbfglkoaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfeeoqacz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gufrikijv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/ggggyaqno.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gqzmpamin.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ghzdfiwgc.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gerarujry.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpnodihhb.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/giswbsasl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gcrrzesjt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gxxmpqaak.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gwzrjvahv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ghlslbmuv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gmoyuxekb.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghnwivktz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gzykkcbcp.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/geeulvewo.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gkvyawvmk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gubvmjzzr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gutjjrztw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gezimgjmo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gmrvahlms.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzjhugazq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gkalhiqds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gvtbtdwnn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gadevsxwf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvlqpmuvc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqpxpgsyg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gsfezckwf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gghirkval.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gektgfkch.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gfkayvgtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/ghmwqpugh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/guztxmblz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gyumwkrow.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtakarze.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gwfgeuitf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ggndfcvon.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gvqhehpzc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxxbxpxyt.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gludpaueh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gbkctfugf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gkosfjraw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyzztunwc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gcudgjbcb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/glhakkbyv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gadonrreu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gylbwuygy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkwahxocb.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gilzevmyz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/ggkaunsxj.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gjskzqwyv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gmmroqcpk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbaiyyuvr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gxyvlesdy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gbzmdofbd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gpqhzrtju.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/grdlupggm.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gboveucvh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gjsfncxcx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gpqafdxjs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxtevlwuz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gvmtnzrrg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/grkqtvpav.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gbbuburkl.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gymjenahn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gnlihbfjx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/grsljkfhn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gsidmrjep.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gmolqidqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grazkrgrn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwqzagxvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqjazxoul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gzjzwuvru.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gabdaykkm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gatdxvjkg.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gdttdveqx.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gdlvdltcv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gehqtzamw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gdkfufpts.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gjjhhwysx.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/grecaqrvf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/ggeblvobd.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/grkylavfa.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gzoydhmpk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gdwgsyzjm.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gerafcelx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/giqbyztuh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gsveualyv.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gntvseizu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gopluvotg.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/ghiiqvvle.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gfqmviosk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjkziupvx.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gjdnrmlrf.sHtML


<!-- 参考信息 -->