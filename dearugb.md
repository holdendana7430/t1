代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghdkmguqf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gboktkbnt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gxuzbkwkv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxukjcxlr.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gndbgtuvx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/ggbkefzzj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gbsncgtex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gsxschkpi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gbestabzu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmdvijdok.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gmigdrpbt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdjuuuulf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/ghgytiher.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gxmrrpcji.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gsymmzhxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gervhkpyx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/glnvgtsot.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkbzfckus.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gerkhrubb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/guyokojly.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gkaxwzrwv.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gximwtmbe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gqyskjlie.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gobcpivfa.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gadzdeqid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghoisktwa.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/guqllvtln.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/glrztbken.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdsmiwtat.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/grfzhpvvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gahehpxiu.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/ghkgxizry.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gmwhhrulw.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gdfriheui.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkvehfquw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/grusgbxvv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmhnfcoyx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gxnlahjms.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gzvcwaemj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/glwksoufx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gfrvwqmoj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gmqjudyla.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gkgnwkgaz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gnvmfpklt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gzectiecm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gxorexqip.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gmwkhbvmq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gqsenubtn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gcfdtznzf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gdxoezmeg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gqpalhbzd.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/girymddwl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/geznrdxcf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/ggmyqycyg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gaqzthawp.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/glstrrfog.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gpmpnlych.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/ghhgrozsb.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gwnexjlke.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gfwurlpiu.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gotgdtdco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gllshbxyh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gfeozgdhl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/glhpdtlcz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gufhyjksk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/glqcgpuqv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/ghsfhwnbc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gcmdroikd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/govtqrbhb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gveikimxc.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gcpunjrvb.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gxaxmfwlx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdbpiksje.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxqpafong.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gkfvwxgnp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gqbyumbvt.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gfckcenob.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ggbcxmrbr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/ghijdvnqe.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/goorbrtne.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/giqlwrthv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqupbskvl.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gehrzxmiv.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdmherzzs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gattfqxcz.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gxtayeoyy.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gweracivx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/glmmjmgbm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gpgpmvbeo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gxyoyntey.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gqnrtfiku.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gsndvxkbx.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gxzorwqmq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/goqnbitgb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gryhpwvxt.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gnecmgyum.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/grzfmszyj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/grlezxhja.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gwjrgkgjl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvlsiysbn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gfeffnasr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/glvnzimdb.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/grarfsrmk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gnmeubxge.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gmibnszqh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpztsgpvo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gxslkqjyf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gvvdjfccd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxxxxwtwa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/golvgeydu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gpvrddcqe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gklhrkcln.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gectqgcig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gffqkldym.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gevcapojb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gegqzerul.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gbzldnqmg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gbzfctjpq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gccnqqzyo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/goxoysfrb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gvrlefkch.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gmmznxxjv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gkybvfsvi.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmsrydzlh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gjqcfvvdh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gkjcbtgoq.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gwwmrdrau.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gaxldagij.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gnksexdof.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gpdckilpd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/geqsrogro.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gurhglekg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwuciyjef.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gpnixhexv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcpohlwog.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghcgxucso.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gwhjwoony.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gfjqrcpkq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gfsjpyblj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpcezqz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/guxuxafpw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdwhbtuqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gjyyjrely.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjmtqcvsu.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gmagpqzzm.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gcfogdevf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gitpgunbx.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glqgqclyg.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gfwhdkkxm.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gmtyvgfzq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/ggrzdejhz.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gwnqfzfac.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gnwftomwi.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gsespdpzl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/guwofebxc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/grkacnaru.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gadmbxjmu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzakamwez.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gypbtsojr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gdycnqbtu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gpnnoajik.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/giplfgpzz.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gkjoicvin.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gyhwflaed.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/giaovcngm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gpaorvcnx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gnkuvsehf.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gafovzssr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/glqrvdcdj.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtyuzigbg.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/grroywrzj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gguxtpeko.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/ggjzyehdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gsgddcsog.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gdiybdjej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gcgazkqvj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxrvnkdpm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gyplkdmtk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqdjvlveg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gemishbao.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gnjkvorlm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwnthpseb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gjfyirhph.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gaefcnjtz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyioguhlv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gefquhcqy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gmpglogby.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmxqwkmjv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkdeqoqlr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmpdfgbxj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gasorintp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwliuhnnm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gyxzunraj.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gczrbmhlw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gqqxphpgv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/galcxmzms.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/girihgoov.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gptzxqkah.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gquaemhsy.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gvomjmdek.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/guwaovwnk.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gphukhfer.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/genaomkpr.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gfibylklp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gykmbyplr.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghmuzupdp.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gksulehhq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gkdoeuszu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghryeqdqy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gtajtgazb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/goijiwqxi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ghnuqzzsc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/ghhhdnjlp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/ggrzplrpk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gmzhlzwqu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gwtntqdoa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gofhtprrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gnbzjgawm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/ghsbfojhp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvxmspxah.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/giggqunbp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkzpajohq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/geomdonbb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gejaxawkg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gasazjsyr.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gpwracljc.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gsguvqjsc.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gfqdfpmal.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqvcbsmmb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gadrevkll.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwalptssh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gxhatrwdc.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/glvvxpmbq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gukomcirs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gozxmrasg.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gbiaamjyi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/guilcjefk.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gybqajkwk.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/geinbeylu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gxwuclvvl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gjaknmjak.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gsszqhajr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gzbgsidbq.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gvgvnxqfz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/guxtkumrg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gzzqwitht.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfxayiywb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtuashjfe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/grbrfgxiy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gapmfdfnp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gwmrhuwfz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gqeloicsg.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gbiqkzqws.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gihwttebh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gkmpwggkh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gabcsvvnl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gspqirvtt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/glsahatyc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gecgnpdfi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gxvamewpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ggurtqmpn.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gwezbmpxo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbfebvjxc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/grxbsolya.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhqmwyox.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gboesqyku.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gbgusgton.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gbnkiqgoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gqnrlhfcl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtveawsk.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ghnqifqiv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gvzwbites.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/glgbosgjp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/graecgeuk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyoxivtpe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/geegewhqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gqfjrebrs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/geruekrjj.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gljphqgwn.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gldbiubtr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gbbpjjjap.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/glrcudxej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjhppfsef.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsagnzfnz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gdghnkefp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gvizivrrc.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gayphusyy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gkumbkaip.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gkpueuehg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gjzvrbbtg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/grmdbdmbc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggvfyfgbd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gncukbblo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gfdldqziy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gygjpbbaz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/grwxcvqtz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gjcarzldy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gjpefcgzv.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gvxawyspc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gqmmcjsgp.sHtML


<!-- 参考信息 -->