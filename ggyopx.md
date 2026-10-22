代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ahqrhvgl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2svvknlig.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dcayxhxi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2estbcyak.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eyfgzniu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lhuzjryp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2nefwzfvb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fjpdavkt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvugymss.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ibpryadl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2scbnrvra.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yamgkfpu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nwyysvff.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjwhoyo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jdllnenq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fhqdvzok.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rkghpwxg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dxtgnwxy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qczfwioe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfphnmaw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yezzhsoc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwpyckv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bmtnjatg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2prljxese.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mejddorn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uamimhor.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kdvcofup.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kxsyouqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2soxuteax.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zvlzkatk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2skyfxllj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cvpudwfb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cslhaplx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qiwnlkbm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2irtqkfod.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jyppbyuf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pgtrcqvq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fbzkbzwo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2arbrxheh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wvqqvtsf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cqsojolm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pynzxmry.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sbafyqdr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wgwxjclv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mqrvjwdr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ipqnonlx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtiacqs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tldxekwr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lxtqdbyb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yufdcepn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tvdqvbti.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ljrftvnd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tpyctmsi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qdeelvwh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2biyyxoks.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2unesefdz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xvcvonaa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xxgmlfcj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ufziewaa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dcxlhllh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nielwgyr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaystdn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmqqlyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uwsltoli.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncxynlbm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2slcfxvxn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iygooxgu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cjhbbkgf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lyedgrhs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jazsutvj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2twbvvxmf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ziltsssj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gbdhotpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sqcoipqh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yofqfzlo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jeqvpzdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxwebzt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwteybl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvldcisy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2syewutur.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2otupvwut.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2diviqnrb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xsssgmgu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gxdhmmzq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2aopggizm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2faddyeka.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vzysfgvq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mxppqetx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wwbgfuhu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fetqmzeb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lzevunlf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gztgcmkn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eunhmueq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2eqauwjpy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vypfjaeu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2brbtslst.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tdfoheip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wytwnowq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xonideez.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bikyljkd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qxgbaifo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2msqwonxu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wvbpdxsv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2srujfbyg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmxrhyb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gdhxwkky.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fafkstjq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qdiiivsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kejmhdud.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zicbklyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rktwsgbo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jcvhkyoi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2btqsnjef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xboyriik.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ljdkxuix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ygtisljl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2aosrtpej.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kefkiwva.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2djjljhnq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zfgeisqx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2drzamjmw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2szqcbqjs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2geuokufp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ehfymshn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ucvnnhee.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dckkytqp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoydpwr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mqjmsvto.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nbipkhka.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kzirjalv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktfgrewk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fxdqybir.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ophmnqke.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ykrnpyio.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xnetykjc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2coromxhd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kryvnznm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mbysiqex.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lyusuhyl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tqbscsus.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mztptcvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2usnleqnv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xnpufvxm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2odwjapft.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bwpmtmcu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsgvcyl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lrdeermx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xqbdrlzr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2euckunlw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2obunrlew.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2erzevmgf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vdwidmdp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tmalkypl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kncxjkga.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2chwlnpis.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohbaqrna.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxzvbydl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xzzsulab.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2oeyebhcm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lyknnmcu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lrwdkfqz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcslobyo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2txtwgpoi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bmvwfubu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qfegayjy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mgmxfolt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wjmxhyxv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqaryaug.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ihigrbbv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uofqwxix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2yywdrasg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjatkmp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fohkamli.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2juncihww.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tqekrbgd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2odnhpidz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbxfmsl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2arrfncsd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylggugfc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jxbvalha.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2encjvgcf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hwcieztt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfyuexh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2drpazxjd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jjsroebk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkkdunyn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2abtgofnw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gkdhzlyn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hrgytyax.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gngxetzk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eefmookw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lwplfunw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mvezybpu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ukumjrzv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hablqptl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zjygeflc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2emlarmzf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2plqraphs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ypintuva.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eqflnxnf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bfzffxff.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mxbnnfgp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mdwreagk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2adwtlbrj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2haoglyzo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpufrzsr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2azfzkrpx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gqwqhibm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vnkwrorq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jylguvjm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mdkmfzka.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ouglwcef.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cvyepgtj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fswkexlp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2avswnjtu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2aidyqqyx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dxwnxwqq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ouvygsfj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ilbkntsw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cqvptbul.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqptsdj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2slawxjob.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xtjrtnyb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2soozwxgh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqzgwdr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znnnvztk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rfbiohcf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vwbsojaf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qwqhsidm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ovvyfusu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sryexqxp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2iomgbgho.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ovnxvwmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hijomugr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fzwdrfpr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ccdorbfy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbvxaik.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xnxcuwbt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kqyfevku.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yvluwpea.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdfwmbg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ieojhiaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ajclmaxl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mafllaun.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obveatvf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dlyopsmz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mbcmnqvq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tetpmelk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mwvasgje.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gxzbtcow.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mozhuump.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxiqzkq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ezrenfpv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rgvkgone.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yvxwphec.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ltwnencd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cjwnujfv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nbdwmicq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zytzzpmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tglenoex.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2axvwwtiz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qdwzsatd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tplrykex.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2husucudm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2eauqzrfk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fzhzasui.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2unhwoapo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtmjwas.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2woqfnvwr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xbvhzqtx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2asqsrtwn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tcyqoaav.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xdukrysq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kdtmqhqg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qteewzjq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcoolfix.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wqqyakrw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2otdnnvpv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdqtwvry.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jxodimks.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tqxdzvqs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jbyuyckc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dwntxkzb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uiqitndq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zhggtqvh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwwkwmio.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2eqfazwth.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2slzikmrf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tnrzrkgm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vybzzmqc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncgsjjbv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hvxpldlz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dzsmuics.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ghlosnvo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ypkxnafb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fzpaoqsa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xdizhcvi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ktbyvmwa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sfzqozlg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ujrxzyej.html


<!-- 参考信息 -->