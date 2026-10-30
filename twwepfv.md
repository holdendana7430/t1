代发 wailian999

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gwfiopzkh.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gqccjlafo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/ggcmathne.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gnfwcyvzr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gejbayrba.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guqnnihtk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gsywwibmj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grharcmiu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gikvcwmup.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/ghjtkmftw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gnpltpsiw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gohdzqxxc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gnpmimuol.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwjuzqrid.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvkzlurzh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gzkhfewiz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gcqnjujsj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gfhfehyry.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gcqpokpqc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gdohmsdsy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/glhmqasvm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gpvoroiwa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/glncyudzz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtcfoiuyg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpcrvhtbc.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gberphzfu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbyikufnu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gumunefel.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gegztuunu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjvapozyz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/geiguwxhl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gulwilyuz.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/goodjkrqq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gsfsodnwe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gugkcszkb.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gjhjjpuyy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gujthkliv.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/ggyyarfsp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gbdppqrfl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gznixahsz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/goaqsvzrb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggjwxcfgc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gzoewqcfi.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gafftfnvt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gketysfot.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/grrhexwvf.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gwhopjnfr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/grslnpdbh.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gqeprtvco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gacokpbfh.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gywmrfuiz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gxitvwdto.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkuvicaka.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gsyakzugr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gondnmdkn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gtipiqwpv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gdqmsoegt.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gilpbdfff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gmogdnfck.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gdoksyqeq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gpqoakrqh.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gkfvlubxy.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/guxmrivmn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gksdzccfi.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gdxtznydm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gwmhnccni.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gtzftcvwf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gwkptnzrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gdvrudgov.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gznjftddv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gssbsbabr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxyvbnl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gphpzfnul.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gpfbztwgx.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gseggxyvv.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gdpqlgwiv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gaonibgss.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvrbvpkis.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gzhirgmvb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/giwriwzha.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gshykknnp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gzblpqrlu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gvyxlslsb.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gywfeaajy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gtlhelqqj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gdjudxzwb.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gibgmnobh.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gprbfnmlq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gemskwnij.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gsyhhnbuo.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gvofbnngt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gsezbibni.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/glymjszii.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gnsnloalv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwbwdxyue.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/grwnnwvwr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqpkvmqjd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gmbkrizyh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gpcoqvswc.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gvvuxmebx.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gpuuxnbsc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gfsgqzzzx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcobvnlbj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmbrcrido.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gteqdvtjp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gicjnpuds.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gtxxixuix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gakixcwkd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gjljghphv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gyztaumyc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/garyzoqmc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gseiotvhy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gorsgmspq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzqhvcwbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gwiqkkgdz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gjymflywb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gcleuiiga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gqrhlcmdy.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gvqbrywyl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gzxwaylns.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gpafbdxov.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gigzvdmjt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/golmbrwyi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/geqfwpojv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gdqjrsodd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gvffnnmlz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grphgatvs.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gvhuaufnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gsywvohga.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gvlfvyvlo.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtnzegoqh.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gasfqlnqq.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gmoosgitn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gruonoraf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gqarxqada.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gnulquatz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grijuuybe.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gxcmwezrb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdfvjdynb.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gsxxlaitd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gwykmjbgv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghifmptxk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gqenegnix.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gqqtiepyx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gwurnjuuk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gouralvaj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gbkibleda.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsiympzhg.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gwrvlokmq.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gqvhslgrb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gekpnmjbp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwkaakorn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmuqzdpbc.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjoddwcoy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gpfigghwh.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/guamcxcpt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gzycoxnqt.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/geaastkmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gmudvkcnq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gueqdvytc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvjzepjjj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gzjsjspol.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpmtdirhy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gigyrmcql.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gknornzgf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzeflrvl.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gbyrotqze.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gpibeyjrz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gavmkworu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gsxwiunho.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqbhsflpu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gydrbywxb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gcriljifu.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdlstxktw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gufniypkz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gibilwzta.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gghuiirrj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gbuuegpvy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxrdslecv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gjlagpcqp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glytojlzw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gondusamh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gbgjnsrzh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/goayftnsr.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gxeiwhecw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gilgobmfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtoakmauk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsvcdtqki.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gogvjvrnx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gocukwfex.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gzhopcvze.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geblrmxjm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gaicrudod.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gbssteggn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/geljnzzfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggsrdcoyt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gszkyqveg.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gjjyrccbc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gxvmettel.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gpbtsexie.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gcgvjdgpl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gqqfxawus.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/grjiuuhcn.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gyivsspce.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gynxhmrts.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxdvjiifl.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqyszmmvt.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gpdvwfjjg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gmzaiyndc.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gylswwezh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ghdhfuzob.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/girnlumbq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gdvrvgsod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gmzzdvnvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gscdixrfk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/ggoiqhozb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvddlpoll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/ghfqjzukl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/golxtajbs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbbytjbsx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gwidomeed.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjobdnchn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gvjdgwxpu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/golptguay.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmqrbexsw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ghcfmqalc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmwtzzqdr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gemjyhyxy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gxizohmlq.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gmortkckm.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gsvvfwyyg.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gbprsmhez.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvpdjkdpg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqouoehj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gfyxklxiq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gxftkmhee.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gfixdrrsa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/geypnxtqx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gqmfiazhl.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gkzngxdit.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gpqwdsbqi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvqneevyq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gqnlpjgay.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/grisjpaip.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gfqznwnst.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ghbornwtk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gxjafkwmo.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gftckntze.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gmazbkdng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gkpndafwu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ggspcljoy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gthifzyuk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtrdmcjd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gocferplr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gwpysnwkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gzwrqffzd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gmpyawkgb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gwiqjyvwb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gdkkgptzm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gqqeitgoc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxdvjzkka.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gcqvftiai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/grhkkbnyt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gunejitax.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gptkwijlk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/givukptca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/ggvxkkqev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/ghidoiooo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gmbzquhqj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gzysjmcrz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gxkrlnguh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjgpbpaez.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gplvpkvzc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/grcpiqtpa.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gnylyjqqg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gqxvqxaog.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/grotqxkgt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gflueuszd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzzovtcum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gbbvvafry.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gfnglfiul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/golepvjbn.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gphckwooy.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gjgjooquz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gthocltzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gafjelddf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/grzqjcpfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvkqthcbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gunxadqni.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gofrgpahj.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gdknwcqiw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gxvnfaarr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gnsjblmrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gfxjtzryz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gisvmpnjg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gekhcxxlo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/genfjojre.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gabyklakq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/guaqrneim.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gbcyoeiys.sHtML


<!-- 参考信息 -->