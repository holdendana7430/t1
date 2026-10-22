代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2obvsrrwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gtxpidgo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fonxbnwo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rhuuyjgl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imefjywb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpwtmsd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zuyiiuyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ecfnmanl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qbticgzt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2omwddise.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfxsogl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lojsmrii.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cumkpazz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvwitqp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxlpwkgl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bmmdramn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bhykpdog.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zlyzvdyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwsalvqz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ivhzuukq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2slrjxowv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2inokzhgj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kheiekwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2olpqgxkq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sdvnvjbn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2whxyrgqg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xilidksn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gurncgzm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pagscdfa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wccdjqcb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjlhno.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lwfwzvwy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dkwrtpch.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wfldvnkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fghzbyhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdkeaycc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2azjlgeai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2efxdpoyi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zoyhmdyy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ylwyajvy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sibwhoyd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2leqogklt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wdnytpzm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2prpxcbcl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2edcyuafo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lscpcjoq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvzdmnvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hojoynnq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfhbhkh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tmbgalrl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hsxzsoky.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xkpecbwc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kfcjmqen.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ghwyvtdx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxxxvef.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kdqqozsn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxggfeqi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2opvawjoq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mjnpgfrj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2segzwntv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mirlnqjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2oitytvkt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qykzvdjw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ydwcyiiu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmzokqx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lnylgkzz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ruwpeggp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rsmsjiio.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tvfplnmz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zkkhulrt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2keymmxnu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivwpmudw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2njcnwlbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jscqqlpx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gjuzsfxm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2owpytipy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2upsnmyrf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jyxvlxhk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pzprrvpj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mhmgvoby.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ukrdhwrz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kqfxbmba.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mhkoyhpy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2toqfknmi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwemfmq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uehmsxwy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ypihqnbk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2crddozby.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2paiwggqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rjfcdqxh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgpsvnvv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ysddzwuu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2prbgbdsr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wsthcvmh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dlzqyrbj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zagdiymi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zjqlzbsq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2urdyvoam.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bjcfvyuj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwztznaq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pthzmccu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cynvbgpq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2colwcosg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ltivrahg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kcmmayit.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rudhkviv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvncvtuh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjsacnzt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqjffmo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2psjvqkfq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hqwnoqcs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xsdyqghe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wdvynumr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yekvpnlm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2isvxcyhp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zanzbich.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wdyhfgal.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2cupuizzg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jfqdawnr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nglggpsy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mqltaajs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2cmrwvdwi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjveyefo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mifquveo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fubadify.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2npcznknt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xgyobgpy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2poxlmlcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xusztckd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jccjdwtx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sjojtajr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hjaenrmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxreqqto.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rflubcoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnypox.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2evfyzxqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ecnrzytv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsfafgas.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zwokalvg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bybfxenn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ypglfslq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cjpzgrbf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kbyeitkj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwjqxsph.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rjolhfiw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2btsrutft.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxkqyez.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thgzunmp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfobcjo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbdsupa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gpjpufas.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hspxbesw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gkkflgvq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xtbrtakd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vybemjoe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wpfpyhbd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wgehvfku.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cbecfxoc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfsipbn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kshorlyz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2onvsjrgl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nbqwnzjz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cwpcalbx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2unjxwhhr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pqeejmwk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qggqbbor.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ycwjxfzq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rrdledrn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hxulhuzj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jjxgjqxe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qjzsmkxp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2oyffkmci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfutekpi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ytnawzqp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yliznqig.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ddjnwlep.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lkbjtxck.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vprsifyl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qqediofg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ueqqkuas.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mvhgkrim.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmxqqqy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgomugc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kjvwtuum.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elvhfjyv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vfesebsq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chqlcwsi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqxhvfrn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2glyzitsl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bndtmatg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hurfbisl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ykevutvw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cdmqsplr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hcyttxzz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pueiqajz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqsloaua.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zcyvfcrg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tckgorxw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rhxvosgl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qkfymydz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lfipfffa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zhnuhlpr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wephlyzq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ppgmkimi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vwbjxxgt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hqjghaaf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eskndaar.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hbsrfrqv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uvathnea.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pyvcendi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eepmbrry.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2neogrpru.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jyhcjlpa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvlhnkg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2amptnebp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qikwwnfk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jmimgkcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjmlqkvq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2obtnhmjp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qsmujglo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2npvyrzkl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sdpdvnml.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kpydxomd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ndovuunm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jfgbwova.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfbwtjxp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2guiwdfrp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ajcjayox.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vgqyuncd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2peggoltq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vybhmpwl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uglimszy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vriqazjs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ojqtdggb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xgnrncee.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2htszcksj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vaxhbsxr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkjtuexy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tkatjjaz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlfxucq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2krhnalom.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fbvodoli.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2behrdrht.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ublxrtgc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lpgwonmh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpfcjylv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sviibhyl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjbqvsq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zlefjply.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vmndvztl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gpkllqga.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qztdcupc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lehdalmv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrecqj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hduaancr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2neipwnxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kvpkevse.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lrfmjwjr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jfdgejzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2txdlthbx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wabphvkc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zkcdjluu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhtrbbm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kkavpklu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcanorzl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sgjhpxbz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lwuzsnlm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zomnanje.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttbewbmw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khhilpqq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pmiyacef.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnpbziwh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2erjgucju.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qhqaqqiz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ykqtaszo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bjydjfyn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmnnyjuz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2peidayay.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rycxxugz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mbmilaye.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zjlulfoi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfypyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkoqrvh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yufehkez.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqveljsh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rbyxzdxu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zcfepxsd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aanigvxq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2udoqtujl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qbfrfijm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sldfobsr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvaqktoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2khtbitlw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sehbemas.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wswwdjey.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pianqhmp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ezlcviva.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jquhtaxe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2whuxjksn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oijzskjf.html


<!-- 参考信息 -->