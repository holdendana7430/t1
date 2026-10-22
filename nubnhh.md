代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gytsowks.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gffqpmqt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afybktfq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yxbdiyqe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nfaujupl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2viqtvlbv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xoyjulsw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thhqjhkf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qafohyfe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2syeljzdw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lqacstdr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wezjlqyp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eayrcuvh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxyclyn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mpgnvafm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ejrioimm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kyjinqzk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzixaet.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2elotsbjk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2truklaki.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cefmavpj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dghvrsqn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jsebcxhx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iiqzmeah.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2krgyrczi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qxxqsuxr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2garxvhgr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2omcjmeru.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssqtewjr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2grphynqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2guqikifn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cerltfvg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rkmkvsgu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xvkttuyh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vuvskyfv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pjsfwgju.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2naxncdwc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dlvysmcr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tyhvejhs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ibqigjjm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oaeqzfke.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fhrbqvue.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdcmgsme.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2upvunrco.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2azhueyyy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwusfpzy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pmaugjec.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ebavvpsu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hbamvryq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qculahet.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2erqfhnzt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcrlwih.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoxcgsku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sxoazchz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgjtfcko.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2syxqqxqy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqpuhvln.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pibbvjzp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qlaolybr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jqqveate.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oaexjfit.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kdnzdupq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtavobx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kofbzgpw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iiezjozj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzogjjtx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cpyjvmnw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jdodimjv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2filzpydz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mzreinib.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gdvlkblh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tyklmlbm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2shskzllg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2prblmoea.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rlhbebhq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bscqvxzd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tqewbtsw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2elkjrvcs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqoubtd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpxjjfzz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ymxpahcb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mrqjunmk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xssxffzx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pisudyej.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bjixcleb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jdhqbpsa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ffuvtwpa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vccwhhmd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zllwstat.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ddddqjwt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxybjgpg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffbucvrh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ucnanqua.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzfcqkl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ihjmyuml.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yfszzgxv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2odqjzhww.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ytrddakw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abnykazn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uwpyfksw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jrwurxro.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vjnlvjxb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uhdbxivt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2khqtspyj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qeqhsogr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mngaalqd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2temavhht.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vljldqbe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kfdfhgil.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vhexpubs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vdwygcdl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hsnibtdp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2whkybqjg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mbukceew.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2icsiiqzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xusrbsdq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwmujtl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bfghdocv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2womylqrb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jodzdqkr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hfmhkgon.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2szvnklhk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mhspwrne.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yjwylgpi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mbxbirck.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2caalppxy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymfwsdgl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sobagvzb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pbzqswzq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lelcsukr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxruxus.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2sscqsjyx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fwskrypo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gopzqhes.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eqedibps.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oggnmmbi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2asjwzlaf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vuuvqhsq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ovdkovil.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ekbprxgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsowglch.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qscyhtph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phdnikpm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wemdfpyg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kwazhdue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xecrfsyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xhqmaabq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eokulqjg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vengmfli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2udmvjapx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kfvguyiw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cedpsnax.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2sgwqipns.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mdvwmqns.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fsknaahp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2srlkwtta.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wyasogqh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ttgipiro.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bupljjye.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgxran.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jwhdbovq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2byjuodps.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ygcsezyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kcwwuloq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xxonhvsm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcdihes.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2voflakdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2noezbxax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rgtzscof.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2olnddjzi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fxgsgvqi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kvfupkvy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dbryuuau.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wpoepmkl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgutdoxq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cchilech.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdpzinu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jqkgmner.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2krpedcvn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ymlvazes.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gbgleoch.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2arfqbtpu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgllttan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xurmkfig.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tppqhngt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cejtsfyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nemlibct.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2makmlrwk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ntdccdzg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffngtipu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pzokbdux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ajiypwqf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2relbzemi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxfzwsis.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xdiyhhph.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvxluiza.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lflfxudk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wanqhwnb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dzrwjtim.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2piswktgr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjknzoc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zofmodyk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aenoqqog.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yckwyzgo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2znogekpq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dsikgymq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cnbcesxs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lgukgywb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hiqvfylx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pccnyvsy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zmwtrfgl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lsyqjhbm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oiojpjms.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uhyvcodr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wqwsoslx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wapfvgbe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ffanikpe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zzrosehf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vaiaszhs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxvpqsre.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2reljfjll.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2swqmrexd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tcqlkzou.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qnzcfprn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nswlcvat.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gyfitmdf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jskbmeop.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2snbmzuqj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kmmbrrmw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqkyopi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2skzhlgfk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2squpxjwy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2scfdfwyn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wwexetbv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ezpmvhod.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xsbtoxkg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ewxeuema.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ieipscif.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rxlyugyz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bqbwdnac.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2saglnejq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vicjgtic.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2exrhoiei.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dmfbcheg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2byobqkor.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2epabukrm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hiogapkj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bymvajkv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2adhdefum.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2amqrtsoq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dufsatxf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sbhrscmh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdwlpfs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aouvjzee.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdouqjhm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2slxknhmj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2omlyqwru.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ptrplwjs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cbmvjxil.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cyupacfa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hurnogpe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kjbcbtdm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jygnidkz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nwuhouwi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbttbyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cellmola.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zsmtnlni.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nkvqkiqu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2agykavnl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kvrgscol.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kbhbpyqj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xuaijgdi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywkkvzmn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zeuyhibr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2todwrhpl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umznlbii.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cwkdgoho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2soimkpth.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ocuboshq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kxvwmonx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mlynrfrw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jwarvmfc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mbjabpdv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kxgtcuqh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ovpuyhku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rcafhpej.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypfvhpvm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qjbjfogh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qjdwxptw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvakpolx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgoobvl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yglihzhm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jetrpyym.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2agtqkhqc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ovbgavus.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gprghbzh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qsyfgrjr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kbhvcgmy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ocfzlfbq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2anfmqsuv.html


<!-- 参考信息 -->