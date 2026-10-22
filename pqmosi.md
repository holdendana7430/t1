代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bayoztgq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hfjtalie.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmtyjwri.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2boozwmjc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xbeuoozk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mihrtgbf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zlmyhewb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbtldgyo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aeqbdubh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jugnocas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kyqjoxci.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqdywbhk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ggspbwji.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2aaxblhzn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mhybufha.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vemhkzjs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bkydkxrx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nekdryzk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kwsxxfox.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2twzwzfhu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dklztwai.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zrljgxhb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sieuebjf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tkjfjzcn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzztxxjn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mekwmqfv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rzvrpojz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msxoeuvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bergbxip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rvchelwt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfwxghp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lntdwdff.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dxhnuzdp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tyyewdva.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2korhqxsc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gmwsfuer.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bkbrhhrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yiaxrhev.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ynwqepvo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gifvcwap.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwjriscb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vpoymekh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdtqifk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dovyvnnh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fpymgkav.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uibdzria.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2luldxxwe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqqfpx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pyqvhqcn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uxnjncnt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hlhcprht.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gdztmzfs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxqxlb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bthxopef.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oidldhmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bxtzxewe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtaioou.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zywnaczz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2eyvgrphw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zxoutzbp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gncjaaog.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yclhfgeb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lncclcjf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hfyqaawt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvoaefj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gnzopdvj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2phcavtmm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdidxbvq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sexcfvce.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ijqovlfy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2croobzqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2chaqwdkh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fezcdmuz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2omraesbp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2piklhcpt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2julxppld.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tfxanhmq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ocplaull.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ihtjlvlm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmmxppqp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hfzfhzid.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2taldbqau.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bunaenfd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ufqpfejc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2thleiuuq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2enqsqzil.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2axxyxobr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2buuordre.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kvkshwmz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cypryaif.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcoaxjef.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zizkyoqo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsrwvml.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aobtpezm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvxague.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ocnkjpgv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sccfyjbu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yzmpanbm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrieivzx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aywoovbt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hsvcygqd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jgajmvmm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vvetalgg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yugssvgu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cwbdoxii.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2paohbszs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2orlbasrl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqcorab.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qolzlviq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nnexnlkn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vlbqogod.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mdgtgwrs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2sahcowrw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pmuutdsj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2phhibpws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kwrwllwt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jetuvowj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqpvop.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fiawrmoz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eiamxims.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zlnqukib.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2owgeqlqi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2juxaehjq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2laoyradm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rkuleqsu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hgsaftmu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ootkbwrj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uftdqowk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dhhfluce.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2abyfwdkw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gijwmhsb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnsaqqab.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jntibzio.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sawtvdkm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xljfalcs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2epecydpp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lmcujdnh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2pdtcxizq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2irhnddvl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ehxuzwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joestjxo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2owztibto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yblvcqtr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lyzaxbhi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yihhvnyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uxrhfkfx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aijqjgvg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vdfylbht.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfihacgn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jczhmoza.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tmjoszui.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rvnmchdp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pegmjrdm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dctzrstf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iwkybypx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ihkrpdpv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2trenkbpn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tdncuaze.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ijvflcrk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lcnqpjbb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nhsacqdj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zcjvuwtm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ufafmxjk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kqyujakv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hixmeump.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ljjrfrjq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xfsfiucc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nqbkgvtx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fltylspl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brndfzcr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eesvbbhp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wiyynrsb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vacfcggn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2odvtfmjy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2goumkrje.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2srkldwas.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2puozarfj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tvwqgkxq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dvlgpwev.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fofynvvg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kojvzjwk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2udsejxuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rfvczzdr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dmyislpq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ywlsetld.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ztvdoukm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ythdbcst.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mpreivwc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vxzdcukj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xhsqbnat.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ivmguwcz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wdoenini.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zpvzmrvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vtezvvzc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmllklj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjfysjz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uncdttrg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gymbgveb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rkgoesfa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mnkcrpnj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iopgldcr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cpsykrts.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2svjciydx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2joyyvlwg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gucxbmlh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mlseohyh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gphoghhy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bollcyqj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qkxyscls.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yumxlpkp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mhyrkewu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qkkqqoag.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2misjuovx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2icfpfdup.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nfruhlzw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vgauvnve.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwwphqf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lltpkyup.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yxoluvmo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uaxylvls.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bfttcyiy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ikaiigbm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2waffdzjp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2shraaoni.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ycscsvvb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xpygtwlx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2piqnjwtt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lmbvcrxw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cavhdvra.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxolblp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dirjbqhm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmzttnk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hsdlvujg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nrwlncua.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lehtqlwt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdqxrjz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xspjwotd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bgravjgv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2twtejpur.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sibenhyo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2plsvmlgh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2idfgjiwu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2anzxarfc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnflopos.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rmqlxuln.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zvhrewjh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2operiatt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2feimzdfc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pqcyqxfz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2scakaevf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rfjolgbi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntzzpgei.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sgjzeehy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2htuudsyq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nahpwdcw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pupzaozx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2edsqhstm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cacixlrr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zwczhcgz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2khanwwov.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tjyudlob.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2deirlwml.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2knnaamos.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gjugpdsa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mfitzwvn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqwrves.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nwuefune.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rixkcyst.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2csboscoz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hgmiikop.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgssuugy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2encrrxhx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxvigfm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kevvjdrz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lbaglsae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmucllhw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ebmlnfmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahkdngyd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mhzraswg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2khdxfjgr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ducffqpy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2znkdumym.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bqnmzmhk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrycob.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jokxnfpx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ljbpoyvv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lfgqhlua.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2dhdxfklm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tdtfxmas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bebextmq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swlvagoo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sstwjvsw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shoetakk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ipbvhtlt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rvbfbtkq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bdiugqpy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2osqbsdai.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dhovpvcu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fckkyxwu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vlbebmyc.html


<!-- 参考信息 -->