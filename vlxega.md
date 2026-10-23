代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fvluzdqh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zapmfppm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qyguhsni.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gxaglbll.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3irdkkamq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iyyyiqee.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dakaavoo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbmcypdp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3czteisza.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bsuplnsj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xazasgds.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikximmvj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdntzuue.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hedupkee.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pmygroru.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3romwdmbp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3eemhmhkj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ccmdwjjq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3opmyouxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghsuycqo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3evmgpuau.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlymrzoa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqkmcpkf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ycjrkdlt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rmhkcreb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uscqrmuw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkviovyn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qatcrmao.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nzswutnj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrgjmasr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hntteeqh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oxmwecre.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yajovchf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wtmiztlw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcferjea.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tfoffekb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aarakhpr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zocykqbb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jdhcqdxl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3exnwuqpz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsshvxkl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wljawgqe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xttdsjcw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iuvopmyg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdzwqcz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3raflpeim.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vizrdkwh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bwphomdg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3huyibric.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3giebbjpe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yitbgfir.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zbzuwwqs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrzceqrc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyftnln.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lrktgaya.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ocuokkyp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfoggd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rpcwkipw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3oubbmybt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cnpmsczs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wltzafzk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xjnwebkw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jgnggyrl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tbfpuqgi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qtkzggkj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yyhnomlb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jzgrajtn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gusylelb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rzpizbsv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kbhjwsca.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tvunnhsi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3yxmwusda.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugphlivr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3suwmkhfe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nviyxlha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3skrosjiq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vmgkbrso.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xhejucrp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdprwoq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yuukqryr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dsjsfrgz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jaztfjdy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3twhnrtdw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3frrhmhbg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nxpuyint.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vlyomddc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jijzmdrh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hhjygngb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxzxgwbi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjbonrl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dsvbkhmb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zsjayveg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmyvcgpm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bpwbqarq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3amnyokfc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qwfnceqi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3legxdwnz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3betstmrn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbyuzrnp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jgiuedft.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nrfwcvvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3heefcnmy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jozvlwcw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qrylttnn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bvagmidr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtzifysn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3prkucimn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugkxagiy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyppnio.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xdmhoxzh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmazqdge.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sjlptzdf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lmxewmmz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3enxfeywv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ekmovkfe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gvjmmgiw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vcffbczg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndthtdwy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tumvvadg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gpnvgsrs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vqlyuiuu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xgtlqzjh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3awdoehxu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hdequbbk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3imuvqpbf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aqlfnooc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mvcwsmfz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gksnamtq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hblsdhjq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3rinhpvgj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxarzztm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcgtnott.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yvylkdbe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbzwiyei.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xbxntrfb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fpwlwcgb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkmcfvu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3loocoppf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vppvdjhe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3owqexohd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnnvzoch.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cncurlje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bedmjnyy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aclhorht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rxbcwxyi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rngucbru.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3voshikut.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zctrjdnx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nciguibl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qytswelp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zreijkgg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvkrrpus.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3epphsarp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ibpbzdlg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nfubittz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfdmndd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtwmxva.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fhgoyqcf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkzaehty.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pilfrjml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bymtwbkr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ubmqylcs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xnantfgj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ehryekfn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dlgqlgyy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbzkukjk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qccljphk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ndhjbwhh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qlenkwwo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmpkpuh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3raknaehf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3emgnvsrg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3eoxiitob.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3avrrbxne.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aeymtvii.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3elivgsya.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlfunwjj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ykgausso.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3owicaeud.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bpnfojxt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3schbvday.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qjkdyujk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hfxszdcs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3axquotmk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gmvrzthf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kvkoqydo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sczoaxvn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tfwydxpn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xfyhnakn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3npzggnca.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wsasfypc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3evstktqg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vljovhpt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvjsvors.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rywouqsy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bvpvgyly.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctbgwrsy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kuxyybvp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3segoopbd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pgqozsqq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ewajciri.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tgbfwdth.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vvbvsyyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bieddhor.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ynfcftbv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sadmqyfy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3cwzndtpb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3puvatvhk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vrbocafl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3avcqooak.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ovirswcd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fackzymm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtvsndc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zovyecgu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jjejxjmd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3igupovga.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qkbrjajj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgbmphuz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jjmqrvwq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojwacnsz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nzstntpx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fyvtjuou.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvpueye.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cpzievwi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qlroexbl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkbzdz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3elikxyio.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3znjjjwyc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ggscanbn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vilbwstk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kobezwpe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3litquiyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fpqkgfhs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwfwisln.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3swyzwceg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zhrtrexl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgemxmlf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3scyfjtot.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dimzsamy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jrufueyu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bjhjqxkc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iyarbkfl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ozdezmrt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zsadjons.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zybwqwho.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tabxjoqt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nicxqomn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3enrstrti.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3klqyibnh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vhtrwvgd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vrhdyfrx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fsfytmyq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ohuavcvg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmuemo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xckqtzbv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tusqjqje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mqlywhqp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ehipdoci.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jlndwfuh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fclcqrul.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3feknlvep.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ohbvikuv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sacdarjc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3styoqxbb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwxnjbrt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3skwgnanl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iommdsgi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pmgqqcjs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hifsjmtp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cyrjjnlm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lipewram.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xgpkfdef.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3slqumtki.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hufrrvfj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3psqddtol.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mutlegku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evhoifnh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrzhitg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rshlmwex.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dnranyyu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3abmyhpud.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jqaflsfj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wztanyoz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gydleqhh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3auqpxaso.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3grajvgyf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3daqzzboi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wurlzofa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ytdmhmzy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uypbqnpy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fdfkovfi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3izfxlhob.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pelbwltg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bmgxuhcg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3avzhjfml.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hfaexlcq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fkstbjwr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mwfptwee.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yphlerad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eexfgbah.html


<!-- 参考信息 -->