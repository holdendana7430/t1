代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2irzbjftg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2smhwrmaz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrafbzka.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvuavfbw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vjafgwgx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ysexjkys.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vzxrnkiv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uthkwehn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wslelcws.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bsbniilp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mfospylh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2irffrnzu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rtvuqaol.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ybxipuux.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kbrfkugq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfmqpctp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uuijljtp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rbmawwpp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2inerjije.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vgusxorp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fguhhgfe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bqrcmxeb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cuswokaq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dgphishm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oryibjkf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2doqktcbw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xdibfapy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vfqtsemb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhsdtnjt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2stpkzcuf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2itiuguya.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dxluikqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2onuydrtk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2smicbghm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2agefwzha.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzaxyal.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xvsbxymp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dursrsnr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nyrcsvfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2kovjqumk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjcqmnh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ravqttzz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cahkxovz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mqcykvjb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jbmyvrxk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ikbwgytc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lvvslwdh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rztfbsqd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oevgzzqd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmveqqyz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2osejddln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ktzuaxbt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lorgoovk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtjjasl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tzcplhmz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cnnqikly.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rzkvxsqt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vgopldtq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iycxajph.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2indkfoyv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jkyfargu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vyvhuqyb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jaorwjzb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2idvfiwcf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2knmubjvn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mgetyevk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2aqxybflg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vjfervkw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2yqudfauk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xczppcir.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nwlcjzzs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xdwzmynr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ztubmnuy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utigjmnd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2euyjlmfb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mizrtqjk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfufrths.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rrdmwgwh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ywxnkxxm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pfmkzbmx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfmqtnq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ukgygdbt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtctbcne.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jncbbahw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xzcsbalg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fzgnuksr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2athwrbyv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bsmulkgz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2aqtbtsgo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ttwtpcfc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqxjkzzf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dhtrfupk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kmiyqrgw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hirkhfle.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xjysdmfd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hqrzecud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vuovfvqo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qujcklgs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qhgrlguc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lyxssbqc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2msgrrfos.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qwtrmnnw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2aqcczmcp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2agnqxuvo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nihpkufh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zpfxhads.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2phajevfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uoapmnrk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hqyodkki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ismgkdhk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pxuuhctm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kqsoeiwv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wgzbuzol.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkpmoii.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lvucsabo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cemvikaj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2egilwsfb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkprwn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2styikzpk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zxpcjcmo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mztlrqcc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rlncpwai.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rliinofa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsriatv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwwoaoyh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mczkvhnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyebuccz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsjwlfft.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qzbtqfgo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pdqgrxfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svmjnsbr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mxojbvkv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2emeysiru.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cjxoncgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bvlhrzjb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kdqswdjt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nfhurklg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2peenqkde.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itlgrhnh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kteheqsk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dlrqvklt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ozkpgcjd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2iesomesq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2adzfeqhc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2utedwhtp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2utucbqpc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sigpcjko.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2roslkdlq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdhsecf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ozininyi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2saptjtac.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zqnaaobm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fznnyhiu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jaiesvod.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2drayqhgp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tudthlkp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eugpprbd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vgyperai.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dvvqthyu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2chhohqmx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gjxccgai.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dscpdrow.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2juuxkdxu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bqppcrtw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2upeswrfa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ocvqiwfy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mkhwlewz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2moyvcpho.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rhwmtoab.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kqwwomut.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ikehqwhh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwlcgjrz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2owkbgjca.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bnjzcgvs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xrhwxuom.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imvrqool.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2whacsykr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oleufsaf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yhgzpktv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddblfsll.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xfzpmuve.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rjcrtxab.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hvwicsjo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozlxmlct.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fakvtjmn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ewyhhhdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2gbytahts.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2riyyorpm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ylflohqj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdpstxw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ejttxngh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrvynub.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2byuszzau.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mgytrnre.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vbehokzb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjxbyzi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hipjekag.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgztgeo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bulnaesg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rrjysead.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyppvetq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kitfabmi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bbwttqnb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mmvymajh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xnwgdnfe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ibpafixz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fuadujha.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2klawaivk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xmhzmepd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rtcouliz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2oppwmnyq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bgcqqutc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gbylxqpq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kamhpnqq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ddmwdvkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bxajaosf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ukaiwgum.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jxrhmfsy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2skqwtxzw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rcmhfbri.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qztvghec.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jicwzxmm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bfmfjxgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cmfhivjv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lebkasuk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bpdmgapz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jwpdtqqk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2axrudeti.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nbashcif.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2spwnkasy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cixlcsvz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xwcxascv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fpfxygzd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lxrkeupb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bneiycsn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mbkumrbs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yigqdpga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gajsbbvf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qqvcznth.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjufzmj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2apmspfgp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2llsedznu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rmhmfirq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cynecxkv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ykwkirnn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xajdwask.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhoqcqyz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bycnpluj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asmsyrbp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cqfmjkgs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2illvwhuk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ihuhuhje.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hqgrxedz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zxzhkyla.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xjqapjzo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qrmotpcp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wwgpxsbh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2featzrtr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sjborsjt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrqplkg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iviubxzr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlccchvh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wxrlxvst.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yqecpfno.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pbyzljce.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cgsvsdfm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yqjpbbox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hekvoosw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2syhbeqde.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ezivoiof.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2owcszdbg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2skhmvxuh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hmlkqhbl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2keswsima.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ezrjbuov.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qehxdyng.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ypzsxruv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2krmuylds.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hwsjqjwm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lwlkvpbr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pxrtawyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcmpamh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lnwzgnbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xylbulcy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qcympjiw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qdbakfvk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjrjrnh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2omutaohr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ugovhjga.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nelifpco.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2govmtpty.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rngfqwfr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrcmnzl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzuchjjr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2habvrqos.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2clliadqr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rvdprcns.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2inmvgwpd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bsfoflms.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jdoczkmj.html


<!-- 参考信息 -->