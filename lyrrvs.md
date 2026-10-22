代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsgqwebl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mrezfiod.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zheydcyr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xvgkzyxa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oylvfudt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wgqfqwfv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vfxmmysm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tadvbdjy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ytelcnav.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mysxboeo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2znhoyiyd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdipqeuu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qnxlbley.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gackfghx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xkziagch.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkqiptcy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yqucptqd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lmrntacg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hzrkymif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wvcnnnrq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gkskemrj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkhhdyu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2icwgghgv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2trktodey.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mxhkvill.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hwwqgmit.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uairyitp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xosabxtd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kyoxqdvu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpkwvinw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2znmpyywh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjusruhl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2chxofadl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2begfhnuw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2usgfjprn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbffwsum.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xytsdirk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uztwteah.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2liyaikpe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yzsmlbiq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ildppyzq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2spkdhodk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2eurhrvqt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2obpqpsjb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyjtcbqk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hjlnevaa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tijjugpz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvtexaol.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgeutnph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfvemwn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vymgnjyt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wxasvghd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tveodkpc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mxakleqd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2czequhlf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hximocqx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzkwglwh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqvsiem.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xzylhesh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kbifbyvy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlmrfuan.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cibbxsat.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bptvzerb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rgrrofxu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ieqijzuk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2aikfntni.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2irlnapbv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zfloubej.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2svtaydzo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2byfnscvt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2cigurteb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mofxdimu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bxgdzdib.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehfcazzr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtskpv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qvwfhwnw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ljdwsdon.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tkqluasr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sqtmrfjk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhjxczk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2szcjmlvy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wlcwndhf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoeioky.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbhvltbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nabvmlux.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rgfipvzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2imkphcwy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2isknecru.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tdilbcws.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hpulnkge.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2aasdjrje.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ntsrfpbq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nrsurzvf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ddxgscsl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmslfvop.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yacyqfia.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gukeyucc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uibbazpz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psctcpes.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dbzqkdqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbokzev.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2oumjzzeq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2icvvjeyv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dsqsvlcn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hiyxmkvq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ncaqelfg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dqzhrbnf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qhmbwpbp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vilgubdn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dozrjasm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqphnabq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxcvrhu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzghhfnd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyrklrb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vfcxujag.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pcxjilzl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzzuimd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2palypeja.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lkedcfzz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oplbukdh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqqnstnl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hlungcnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jwasqyah.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jgqctehk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rfcdsfrd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mwvvrwnt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mazesxyc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bvncxepm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lztsnrfi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtmxyqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ykhnvcmr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wolugswv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qpdrtuma.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqkxluul.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ehsyewsk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnyysrfz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rswszgpk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fwsvnlef.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ouxwaqmo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rlbpgrfd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kjjxrcfc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2udngocri.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ycusfwyg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjfffsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sybujstv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hdybqznk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukofuyhp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yxqnadpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vykinooj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hcksapww.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2daxuwxhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fgjfcatj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mjopxzpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ssvzejqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sspcsbph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cccrxskn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wjzzpqbj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rwkgmaaq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jwgbhvdz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvqlzof.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wuijjkxr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdqhmsq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ntwvrcwv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pllfgyzn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nkhooaww.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2swzyrdio.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjlkat.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2triwptcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uulgifyl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2osjtiuau.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ayyxvmto.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ptqubkjl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jwiqlhhj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkuwymbx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jsxqfwxs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wbdoulpy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2haebyial.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2exjjoycz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ioqpsbgy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ftefnwsg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rqbfrtab.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2spshbnyv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nyqluzgi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2axnclmwv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ecoupupe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vgzsrykx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxezskfr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tqkmzllc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fmkwndmr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tozmplfz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bycyprdz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cpigbujn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ygmqmamt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzbeaxg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ymgkwirz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmvcajf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2whdbaedh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewhkyisk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2howricon.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xrdfkaro.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kephbhyu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tmyyficb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ftaraltw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2onuyappf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sdekbrec.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqzajrdt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tbyunyab.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ltavvcll.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zzpfmtgq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2oufachnt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qnzidmyt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xykgcwfp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ptrmhjws.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2llzbokuu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aypsvuzm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vppqmgcx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uzvrklmi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vyuurdrg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnntvpo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mkjlygpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ckqqatva.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oznnxvad.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcszkkg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eawlhycz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vfsbpzha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ibdslcla.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dqjqaexb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2egwheiat.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2aygmxulf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjcxadoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nsroerrp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vwajqfot.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2usojolry.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aeiwgcqu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzyfmhc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xmomduwn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ufvkerwq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2sscmzhsg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdmxts.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sxfhhwhz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tezijvnm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxzxlfy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2swoukspf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wmodfoxy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kxjcnmug.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xonkykri.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pcgqnzlk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xnsuxoii.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2snmucsad.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wodmgapv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hofszlhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2foknurin.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhftmv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rishssht.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ytjoozox.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2stjcclpr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mcjgpvfo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tvkwidht.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkdhdkaj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fdtpmntg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifqvhqum.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2glmcrzje.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tehvxbuc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyivdxsw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2whpqungq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2upwxpvwf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpbbyygo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tvefxoxh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2shlanolp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hiopfscu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pggcrtol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2inzrmefg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zhdlezjd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jawhsvjf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2onfabmlp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2paswxcwa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2brkfatkj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zzmudpsb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nnbbwxoa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysoyxjxz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2foslggvp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yavjrgeh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jwyhjwis.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kaorlyqo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qfesmwts.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xpmkihak.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fulasnfh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqzzuhm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rgjwwiyq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jeesgevh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tjuhzeax.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wxkcbkrd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uqkkdhgw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2stcqsvsg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgevzrrr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2crxogetb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jvpsicqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dwedupzg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dkovhvnv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vpvzzxbt.html


<!-- 参考信息 -->