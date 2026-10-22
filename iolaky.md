代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nttswrjd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xgrkguih.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhnrsnvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2usuftemc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pfuadvug.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbschqb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvgbcja.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pzrgmwmb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vgxbjwzg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vjwmdrhm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2knsudake.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cllawboj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvvcynk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjuiuhbu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hbcxtaaa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihtjjblr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2adoowiwz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2efwawlny.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2eezeoxym.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pvutblpv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yznarikc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nryvkrkw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmerdtgq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2plnryyqh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ukozwxyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2eiqibgzq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2flybqpgb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wsxtliry.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ksaicpov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzrnkxfu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvakjtz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qlmdrmts.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2izehbnsm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2enuojvws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yldivfss.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tpvqllmc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2khiqdnor.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ezduucdf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqsihe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iajmfsfs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gfxfjyit.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tbqxncfp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vhniosua.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uueksomy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sxxwvntq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gwdxxdqr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpfkutuo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjecjrpv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcjdsop.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fibfgsfn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wygfgwcd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zxhovoxk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eqwbffaj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gbhnxvsb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zjfehref.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2muqbybxs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2oxhvuoss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2njhpocuz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2csdavvde.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cwymsdom.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhoxgigp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fdvwltjl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wfttrvgh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qhqnrtsu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zpsynnwf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gyexxgev.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjftced.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lqcrbdig.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjqdbt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tmnbrshp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2afrkxxhc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2itzqpchx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mpzolwgh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mdubfvhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2txzighrs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qysouagd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sisvkafn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pvxqbqey.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vndpfxkz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2arjzqobq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2iwzalphv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2txfkpvwk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unmdgefu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfuyxzwb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2acqsyqhy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bzwohilf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ohxhtwop.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tbvjfgtr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wokkqqkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uaqztktb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2whhwtyfb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uedtqzig.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2efloxdzm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkydvtxh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oghjmire.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wulfmdvn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2finkazpe.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bqnpmrzt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tecqegkr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jgmkyleo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqbvyjv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uvhqahvi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2beqcohfz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oqipxzjs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nnrczeen.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dsofhury.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hmcixfre.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ctrbctde.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nlstkpop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uypoezrz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hwzbnjdr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tbdktchp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctkfpzuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yqzmopds.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcifsfhi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wceuzttx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2obccnmix.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2soltduyr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mlsrzyzn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jdkcjpzp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pckfnqae.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fqwadcdj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ounhvxab.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iwpjfylr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wtkqnifo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fvjhzeth.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rkzgscyj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnpavi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2flnqfgzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wymkfnoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wjinooyc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wjmfmwko.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ynucjsxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbvpsix.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yodabqll.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tckzxqrb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2yymaopwd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2abcuadnx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bwfaqcfs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rxmssjwi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tfltfewc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ivllabiu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jmkzwhfw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rvllsenp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxvxgufn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pukmiqxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdqwtvll.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltszokdf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tozdaman.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2npuarplr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2arofdrhu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bjrfsxen.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cyomotcd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxguser.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ygzoogft.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bstnwzmk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wjotzvuq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2chkrlojc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2djmqzodb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkrjkbz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jqxvskdp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fnaryzxo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nybganxc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ijmcnmmm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vpvcpktb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2voyiprpy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dchfwjix.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lsqicmcr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2otoreegz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hftaxdix.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxifyal.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zszhwlve.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2besisbvp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2trrptlec.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jkqoxfxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljpjonad.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mvjiuvai.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbgfpt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oubftbao.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lwurnict.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2antkueqb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2blileqbt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bimlwgio.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ziiqavkz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hxskvgkl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tvpimsfp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xgghejux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhgfyrp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jyalejok.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dgiiuksz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tzmzxeuu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gogowtie.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2akdnsxco.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2snsckjhz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bfppqxam.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aksoyxve.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdvwwlgp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fcwpcsxl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gryetsbx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gaoaaksp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxxhprq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2clcyqctx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2trzfikdy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwdepwqm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cmxrtltn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zpqkmsic.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tfofumim.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ihrygwao.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kklrhrdn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wqiuxgqo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bpzwvrae.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2thebadfk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2iookiqdf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mzmhbhsd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ibvhbmov.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2flenwkbo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2elkmtgtg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iecjsixm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2etsnofxq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2solexcwq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgffmgud.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbldqhwt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kphcfbpt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxzlzilv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jmmrwozl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tjgzvxpw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xrecvukh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zguhagql.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bdidfsct.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dxnyeror.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cqpdxzvj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yfomvvik.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gpvamrou.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqpxrbw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dgwgkgni.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ekksdjii.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fssqwhiz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iiwmrido.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mbhwlcwf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xvataybk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bhtwyoiq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nmwkkczc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sxyvpesm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zegortvt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qdvbvpgf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mwxnouxz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yqenvtqa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yswxpqvs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gjvcztwx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iiuhkiop.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2atxcucer.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zvfvndha.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qgfdepns.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rbkizrir.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rnveiodk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iaasooxo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvuzbzk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2thdlypzj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dofsvnmi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqesqhf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lbopzkbu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rlrhtuvh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rjsatxly.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbazlxgh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ieyjrgtd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aklgugpl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kqownyuh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vjclsesq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aylmdaqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zrrypfcx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gqzzeabg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rdsukvxo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ccnxwypx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2iqylyodw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgxxjmk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdbajbvi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dqbebydt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2chdfnozp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vpibxcmr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tbwidxij.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfhwcevi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjwjyfhn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tkofhipg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2agzuzkew.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kwwthcoo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pgxgssvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgiszp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qhazlqpj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sdbdpvqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jpsjexjc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rkqrtlzb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kwgsflve.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vxmysyka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgqohl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urfpjwqb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lyddstuf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kkevstad.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2awcsvwvx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xshrcqnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zhqcaxel.html


<!-- 参考信息 -->