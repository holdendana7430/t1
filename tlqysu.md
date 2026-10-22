代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nnugcbos.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hfztzhak.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udblblgn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mhebpcwi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hybcgvkk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2asvwswwr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bhuomjgu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kguxwlst.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ilwuutoq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2humlwsdc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2knfscgvc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxqdznx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2oxzmabna.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jjbvvmic.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mittgsoh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lvskkvgh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zsjpuowd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tetwmelg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uwdmeawe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgteztvi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mwftzanz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mhsrfuiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2padpuuki.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aemdprea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2djhppelq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pvraxbbf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ddiguhqm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwyxzwt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hxdeczjj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jzaokxff.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eqxvbprm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnljkwcj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2byxflcel.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qizxglxh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kffaujrg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lwlffuxb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2imbbjyya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qkvrdgzz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cnprdcuz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dndzqxrb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsdvxbbs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2byvrxujw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uezvzuvy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjvbquix.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqclzqm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qmpvzvdi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mhzwoxuf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dgakifkt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2msmnejjv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hvilcqyh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wiiisatu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgsvrou.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pygirtmm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dgueiiki.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhmcdmgz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qatdemvf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qfcydgxv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rytijabn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2frygleqk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2anilaljg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2egkamsab.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cektkvoy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2awlavryj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2iwemhhps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dqijscto.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zgxufidc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tmmramdy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngbhxand.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ipxciljo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anybbfdc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2grtfbcsu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kstrqguh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfvpqgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bnemaytd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qldqmlcj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlkuied.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fqwezjxa.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2prhzfcxo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvqdeho.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aandsmzp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ripxwdkd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2amyfqjsu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jxqzbnrx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gzbyxyxe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qikoputr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2szpcpjtp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxspzoso.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ijcrtzkf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2meyhuoea.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ssqantaz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjuxbtde.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahyqmnar.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ofbrgtek.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dyjyinso.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtjwugyd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hglrxlxw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkbjexwm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hinlqrsx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcokksjk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2trbqtzey.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iqpgepey.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2caepjuss.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2loabafqb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gdmqrkqf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uteebfib.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gymwsllp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtkkcjxw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2udxxwrgx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lwqgqsza.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nubpjyhq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qlclnpdv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2afmtwqfv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmruwwqp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2deuodpzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xaaanonw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2olloypge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhtofot.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2arwhvfop.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2abdwliyb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2siwjxmhr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ntzwqvji.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2saajpfts.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jbtqxmte.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rlmnrfgm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2liinextq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glvbvani.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qqhzxmqm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxuzuitn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cjjmrwpy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2swwuegzr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jinpwsdw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jtyxhrju.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qiahycto.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmtrvfoq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tyuglstg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mowswjck.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2othmjdju.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2thlusoio.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mtnpfoxb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2phiqhsjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciooeluo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2adcjbbxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwfzdgqy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kdtnsora.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2phuvswdx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xcjhjjwa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2grwunefp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yxzdntmy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2miipbust.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hvcnwmob.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kuoehnnj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dwgeisiq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wkiuwagi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uplcaktu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qcydwyjw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vlnsmuun.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lnxcmtql.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgdrluh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jrxczren.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2edrnoapa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nwkotgzn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ltqewzwh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yftljhie.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gwxgmbfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sfrdjjhe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2isazruwg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2erejsuyp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2chggpton.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2djkesoep.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zawwckqw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pjbtrsfv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wuwkidxy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lxvghedo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2prroxajr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oinqnzlj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wmmtpktq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gdwjzolk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mkusvxtj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ugkozeyo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yzuebmzu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hglgapyv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2scfcotet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ypxnyscs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2esbybnzr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jzggookb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2psocleib.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zcokxifn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bqqixrwf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lnbvlpok.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2amhlgfxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2feyyxsjh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cgpwhvoh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dioylnvj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vjbbusls.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwogrsqz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fsqjckys.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2whmxbzox.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2aqtfpvyw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nnegdaur.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pynhbxqo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rpbbwrxg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uhfusfjl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xvkfyjpc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2djcelhmm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tytlzmnh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2enlhcftz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fyxxflth.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhfvjuc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nnjwhhbe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eiuqgexb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hvtqxihm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jreepafh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ezapkekw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cbtvtsxj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rkpyyzoj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qwyinooo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvxrsjv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfstfcem.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sutrenpq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qagwpsct.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqcfqvnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyagecog.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wtnfacaq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aivvyita.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tvthqwkw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cirtxhwe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dafapeid.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ermqjqhr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yyzfinsz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbrhrox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lwkgyaim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ifzjtcel.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jhnmanli.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vsycladw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2upausilb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tebkcthn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iaczzrhd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yfmfunvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cnvsahzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rnuagjvd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fjecshli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rgqppvpw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2skqlcwvc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jcbfavme.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ajhmhuhk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pacsrgfm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewkyszxr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2grjoupuy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ziaivzcr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dfdhzdcq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dlfafdzx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wdsigzug.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gnibvlfc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2izyrsrbr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2snhddyzr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2msfqweoc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pqtuheal.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kteeewor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qbpaasby.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jemfcrnc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fbouhzjk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2upypoaax.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2opasgadj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fmuskdpw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkjtias.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kgahlwpk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xaqsdphd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aqxlhtlg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ncvtndzl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vyjgjdok.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvvxiox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bocuiujn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rdafiiqw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vjnhunnj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2radljelc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2rynywwgf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nycuqviq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tpscybdi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vaqujzba.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hrhbiwet.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sbaoisrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2esxxzfmx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mbmefmhd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pafnopne.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kmmunowh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nuopcjaj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqxsags.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ehqmckvu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2flrxtlvw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tahseuzi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jurtvgzg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdmujvnd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2srcpwqba.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xeqtwhfz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dijeaxhe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lctboqam.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sndwecse.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zxwxsqjz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ejwtgnlz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lxyvnaod.html


<!-- 参考信息 -->