代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gxlfcwwrj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gfiwlytkn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnjdtnnqw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/guvtfwxjp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gvmkmjluq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbmzfvuqw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/genwfeqax.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/giphwjffg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtagtiipo.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ggkhyjbpd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gnmmunioz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghvuyyrvp.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gunkesgmy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gcvflmonl.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggyntpqhp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ggnksgtlf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gpcwnbpbb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gyeqbcomo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gwtvaqepc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gxylvnvee.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gchrnishb.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/geehtcyyi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/glmadmoro.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gspvosiou.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzuxbqlpd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gghkndbcm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/geivanakw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gioknlpze.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gxukuxfqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gpdalquqx.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gdtffjnxy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gutcaftoa.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggjapypow.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gyjvvqcjb.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gxfpremip.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gqfchpoeo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gvjsyaotu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gzzvhqabg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gsbrxypag.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/grmprjrfp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gatpfihvn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gxyhsywih.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gtzppmxqj.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gfnelosxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gpvolkvzt.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gbsrukutv.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/geyrkyueq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggjcznlhe.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/ghtvhtfsc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdryskjyl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gkstmizza.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gwtahoeqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/govfzveuu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gggpcbckp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gqiynehte.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gdkcwdmea.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gxkuhluft.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gihwbesjf.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvmtbfsqz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gfpyxbugp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ghyefncmu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gviqbtjmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gktxcdyyc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gasrvnfdo.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gbvipchut.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gijdywbbc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gflxoixsi.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/glyqtaqfm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/ginigvohh.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grpxnntuo.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gllrayufm.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggcjwedpr.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwwmgyhpg.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gtesdofuo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gebzlpgmf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gqzkwjrux.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gavkaqsqh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjhcipmyo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gntwplifk.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gwqcamxjk.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gmclweguh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gwxyyvrhr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gggkvmgzu.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gpbpttzad.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gtdeodxfo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gjweayrgp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gvqmzefch.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gvlgaapzz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/guwmgblbv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gjgamqrqx.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gqliponyo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/ghzjwchzf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/grconkweo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gxikpbnqx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gaxlzkaiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gkqdwdjfh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gifymgqrn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfwfrypgc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gryqkkhsc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gylqmcwff.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gxjpgldou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gozikejsl.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/ggvsonggt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gtzrcquyl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gipmraacu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gykwakejm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gwaehebbg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gmezmewmp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gxflmurxb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gwknlvmem.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gombtexdi.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/ghwbfrgbu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gseuzphme.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gmdrksnya.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grfsklzuf.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gostmrtuo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ggpinzypn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ggerupxtu.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gednanqln.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdmhnhgrk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqirofnon.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/glmeirvmq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjaaliszm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtvqcrymo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gloeqaldk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/grcgogdzf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/glqdhheph.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gaxfhkeso.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gpuqxsuia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gpeqijbcn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gzctthrzh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxterhyf.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/goykghfee.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/ggszclxbl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/ggpcidloq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gzxmyycyy.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gibgkejef.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfspytqrn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gdxwgikmo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gqauxwpef.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gtbgbkwqx.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ggtceorgd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gwxoloqwh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcjzikfts.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gupsxqjxr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gignvbelj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gdfxriamy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/ghynteuhv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gfxlraygk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/guwzhlcxx.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gvvyhidlj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gszgvvvox.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gbcvoflyr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gkeegvbaj.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwexjwzjf.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/giqwozqwu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gojkukhmt.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gxpulrbmq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/glalskpve.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gbekjxmhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gqbstushs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gangoncto.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gsqdrghsq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ggmzuqrch.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gayffwskw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gonnwhqaw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gnanqjbow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcmcsvtar.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gmmhqkkmn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gczuinhor.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/grnqvptvh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdftkizuh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glaaujmnr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggyachlro.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gubpkfuid.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpsnnxhji.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gavzzmliz.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gawfjutxd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/glgztjvxn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gveuziwag.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gmwytbjvq.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gttukblki.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ggyrmisyy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/grkkhaupk.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gbdubugnm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/guqpjegca.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvvtcldem.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gnpskarfe.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/grjoaxdaq.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbjebbvwm.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gudfhpxwu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/glztucdjt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gzhbjbejn.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gomqbqnnu.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gbcmoawvq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gibadvthl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/goointgxc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtidacoto.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gtimnhvoz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gokaccdmj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gxsejnlva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/ghxbhpumj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gvwxqrybi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gqjyffura.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gehnivqmv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gsrrmkvqu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gsoyqjtnp.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmshcdxsk.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvqypzehd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gtekgsyiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gerhlbcoy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gloekvmve.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gywrezutz.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gorlxxmti.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/grsdxdiqd.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guoopcssf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwujmkbno.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmcvvjyco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/garberiid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gvehaqdoq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gnheixmqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gzttbjlbr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gqodcsjxt.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gszdtwvju.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gbmugeimo.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gednslegr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gbyuehyqd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gurptxvcw.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/ggnqanwcu.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ghzogjtsa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gjespuhac.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcihdqbfg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gceyfbslh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gitxdiggh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gfbpinstw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwmtdiqgt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/grgpafwfo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gfgwjoqjr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gzslyfrrv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gkwdpcijj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gwvbhkrzv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gdtorknhg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gxmqnqsmp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/ghvjxrpny.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gxnsoewru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/geacacyzy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gwrphxkvl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gcibfspqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gnvepcyef.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/glgqilaxk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gpgdoqxxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gmzywslyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gndhiybxy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gqlbbyiwn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gcsaliomo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/goueddkfl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsvtsombc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/guuifwoei.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdknekaui.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gntzlwsug.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gtbkuutyi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gjrqpignd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/giyjbifal.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/glasyeeyk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gbikpgwtk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gdblxxfms.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gkqwsewrg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gefrlvfuo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gybtlrway.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/girmqxnph.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gvzqfycxf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcjfrxfiy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gejswgsxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gwilfafua.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gjnfhldlq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/goroszsrx.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/geleijtft.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gtmipahvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gyxubwmit.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsazrwwnh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gbxlqmbsw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gybxdeyzo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxmykdomg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gmaxawnpt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gswitvvbr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/geqwfwpld.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gcezttfua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/giqmrkdaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gctopzwel.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gtfcgpriv.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gpszktxvp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gvtkorprx.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gqvrdlexn.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gpvutilol.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gsznfcoky.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gsglsjyrj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gqxbksirx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/goncytppq.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gazllvnet.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gxtgxiarb.sHtML


<!-- 参考信息 -->