代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rolxzsib.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rclbdxsf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ufhfrvsf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfwteaug.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmqdhef.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hottcdcz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cvzdjalx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyyusgi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjilwmb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pmyqffxn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bzvprxef.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cpwqilqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oczmfumf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vcflxbun.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2phxvutio.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glvjxlfy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ysykhdfk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zxhyeupl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cvgrnxmk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tgkhwrbb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lblucrfg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2medhojqc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ijqoivqi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dykuldkv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2iilehvtb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aprzrkyt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nougkkat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycufnjfv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2utzattck.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2slbbiarc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2crsicyhn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zkuxzkvt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vpszjiru.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hgxkjtex.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xzwbqgmx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fkgmhegd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oeqotura.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oweceeva.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bbqmuoov.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zdxeyttz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqjpzcp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2klkgniku.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2okrzdftu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xkwxioue.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ocfclthk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxtajsg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wzzscqhx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dofjstxg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2shwvihwz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gxoodikv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dhfeijyq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aftmchkl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpxxcyr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2patuhpzu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvyejta.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2opsjzwbq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qziblorn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2llbhddgo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kpsqmaey.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ukwmpdza.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yxcmyoyf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpgminlj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2faymiaxj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2krhhrsfs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2frykmkar.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvdonta.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2stgbspvq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2icyhqxrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2guuzndna.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gmncikvz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lmukiswm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lvqvgclw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2usarjblz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cpowlpiz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avxyervu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nazhuyew.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ccdvlaqs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bxrifhhh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2teagokja.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qpuvhadx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ijputgtg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dmnjiwcz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdvridgq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kjinjkyy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fudbcepd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsoecy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdtmjew.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2faznvfbm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2icbdfhyj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2avrjymlo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rkyslqco.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bzzvliya.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tdcshrdq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mrserfjg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bejqgklk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gvcnxybz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fmwdiyrr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qxtxzxwv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2itjdgevd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ldlvpvof.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2zzrvwwsh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdnrzik.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2safuubpj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxhedjs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhglrmt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tlogqxgv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xptbymdv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tgkqvqgu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtdetzd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ixwfegnx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jkorptel.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2phlnidgs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ujirktrp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wpxptwtg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yeurafeu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kkdbtpqi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xwryjume.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mtuwppdh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kybothjp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tnviilli.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gnjvmvef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zdmaxbqq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hitwpjxt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btttupqn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pxsdzucr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2udowyjgt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2blvcromn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hhkyfmck.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fotdqbyc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wjkalvvv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2juwhjfjv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dqyztrju.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bkevsifq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukmrjhnx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ecuzzlut.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iumlkmlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbkkpvmr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zfijtyxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esfhdolp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mfmxeywb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2npxwifvy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yuztscjf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwiuggqu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2howxiinr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hfurkkyf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrkrdcw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nwnwpuxf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gzzclpgq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hasaclft.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uvoreiuc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzbwebjk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fpvhemyv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fxjlclov.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpvqak.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ptqggrcu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ohdrcodf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hnkljumj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pbfxhocs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wvdlnkmc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gkigdmfo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2efxymcyq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2alwmiqyn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cldynajg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2idcawzot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qpfoherg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gtttogdj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2csefnmqy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mgxwzthr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hdyhfdnd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyhbuma.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ihhillxc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tzrmbkry.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tywubdyy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gjyexmws.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tjyajesz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lyuzshhc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nirwrisv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tlnajxvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gifrfish.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rghcvfgq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmysriyy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lnfdwnzr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ebcpptdp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2roqcouit.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2guzmzgrq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uiaabvwp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2deexkumr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2goipzibi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifdoxxfn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xkglybdd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wtyhmvmw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nhiwmfbm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ingtjmsh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rfofvejr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ghgeuopm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pvyazrmn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xnmeplpd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2asguzgie.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2osgmdehq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wbxnyqzu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nhzlxczq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ayrhaeld.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2csyctyrt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pwenydqd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vczzxpyj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xejobadv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kxnfwgjz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lapqxmfg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nsvbujqu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jhanveis.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkbstkf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2esbhyqei.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sselrlat.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2llivuonr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vzowkcxg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hqqchohj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ivzyclzk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rxyxkpca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qiahqrqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cnrdhlnm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ciuvcqau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2prrhfyai.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dzboutid.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kyummoqf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2auwrwiij.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tztaejjc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eaqvdtnk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gkufdpug.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wkkfyfde.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rvoubpuc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jkrsbcpc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ricopxah.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jqxwliet.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bxvktfcp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2upjdwvzr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rudvvwbo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iyuptzhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2raacoczo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2asxnsvtn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2epbpvesh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2eqampktu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffqxnomt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hujktygj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wjnaqcuq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ttagwnmj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2exmrpuwz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2twwviesf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pmefqjgu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2txjgpwcx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nabxdozg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnpsxnxh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2enzttppr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mmaaaemh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fpmncxuv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2idqeqeeq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmfppamg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nyllzhqw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hmtkpssb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezdmarap.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2odaclkxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kfxobqzd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxvaukk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ryczbbkv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzrdzkze.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hujoxryp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2njrwvpvy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dnmozlfu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2izppfegp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xciscgiq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gztxhknx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2eccyybvd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2awyvgnme.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wvhjaxsb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oknposzc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dpfhlhpk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eepcthmm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2geulzrwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ujrljpyd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dsaqcggm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2usbuyinr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ewbefjnd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2szylyyzo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bkhfgfbx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pzyrlute.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2josauhdx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ljldmkjs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clctfmmv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqncuhdw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bnaulacp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgwypx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gzffwudc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bqpmoplt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2awxetrus.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wssjastl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dclqjrox.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qyxcraob.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwobdctj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cdjxpjnt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kefxlqxw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2slylcjml.html


<!-- 参考信息 -->