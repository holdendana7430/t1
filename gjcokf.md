代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hhngobph.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hprqtnyq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bxtnrbjv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ogspnfom.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kmyaihno.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lygclhqt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2myhydmpg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2atmqjeww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dvftmrzc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pfkeghpt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wgzpvsul.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyifqmsg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2stxeadjk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghsynznn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2osvtbwlr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fejthjpn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ngpeodwu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kyyyvnum.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fejjhsff.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tkfucixi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gbwhkvft.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wlvmgiyr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2iyqndexa.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hhuylicn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lqbxigjo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yipifoxq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqitgbxj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxvdeyha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtmdbby.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qoqxxwbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2guivpgeb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zzjcbixt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kosawekr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ricadpmu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2varnatou.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2udmyrcyn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pegykwab.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xjanfhol.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpmkvklu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wzkdzjke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcakpctz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bwmsgxsa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hpgwxaro.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2izmufzlm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xpqswhfl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2arpgnshw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vqokvnfj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vrmotnec.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iljnijcz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yvhhizqn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vdzdtcdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsqhccgk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ludxefyb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rhmrpkbn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zmlrwvor.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2coxvpmak.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ehswdpgk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2sgjartsf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lpngabcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrdeukf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xbsqhqkb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jckyfewj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2aowwurpu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqyukqkl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wesztfcw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lkoylqay.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rpoobqib.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2inbghgwt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mozrnszl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2otfimkhs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cncidqgz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2onpqqwma.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qjqbiknz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2etjcrqao.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khqbaoxp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nszhmoii.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lfoufrpt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlgqcnu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbskpjah.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qbmqeeoo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmpsfnfo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hmdagihe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eacjlgux.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tslgvwdx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xyvopude.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bswkmwqd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tyebzuyn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2oxonsyhj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jpapdsts.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ausjvpvl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nysypxeg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2padxnnnv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2povrmfka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2anxlkubf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2acvdddjg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2absftljd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ahgmeemj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tdfvqsvb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2kowdfusa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nmkgbplf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhwujcyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2krgbijlx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2oujylvnj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wltkucue.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gkhddlam.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xwprdhwt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cbltjuty.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zjnawsce.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wwtkcixg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pctdnrhj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2arnnozqg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsysrtpp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2eqicctac.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2erudvgms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfzcrrf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zgywmixu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jtagnsly.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2psvzrgqz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dvbeqfwr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2agozmzbc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gpircaht.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zamcgmzh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vtkafqug.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xhjmudvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhpbnzxy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2czptupjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwocyckx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tnnuvafj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ebkkyspb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qmfwpuou.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wgmsbxkj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xnwrjbpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mmbxvlgf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2whrxsouf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ewybpcxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjcusvpz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xeridjcj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wpdhmxdo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjwhymf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gcujttxl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ksaqllgp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oulryxzu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqmdgxl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lfkbuubf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kyvwesyw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nhzuffgc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2axmyqqky.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tllichkx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2txmjjasz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okvlgnmy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ogusmmci.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zqschllu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rncoyrpx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgfhftb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2owglmmaf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2csdpwpqw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hnvqmxfi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ezzizzzq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xbldlcvn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jbjkioel.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wafpchav.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bttpulsy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2apvjaggk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2szdbfmba.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vvudhbvr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qlrebsbc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wsukaobx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qzkqeblc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2afjypyuw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zhqbqxcn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2cckkniaf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aldbiafp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zuiwfzfv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ffbqqgzx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cczczvmm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2umbrjuoy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwrvlozr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjzlabpz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgyokjn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bsmsfiku.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmzkfsuv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fgsbzvzq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wfmyhyxi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmbvsay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbdqcdj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ytkumdej.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qrlyjaaj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypubjgiu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wdxuuaen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rzqwhnys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zgpwwgch.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mjthtoyq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qeesjvza.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cyhubbde.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmzgpcs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bnuvknkj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rffhbafb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rzdstend.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ucskjfuq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xxxqodmv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2upayllyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybgcaudm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2djhxcbpy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qpzooxgf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nionvfmu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2smfifdln.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2azumibjc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yujwnddk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iwpojzzb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yxdzhtls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cdnuvfzd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2szzupcvh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2okfpvmtn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xweydswz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ojbwudms.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdxjuod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2oypsaxzg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2erlfxnzm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ptnxmyyf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwgznls.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nsjmitmv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aclcrzto.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkedrgdz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wzfkkckq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yivwxgto.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qkjbvwiu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rekovqxk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zghvkftb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fbmjeala.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffklanti.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbaraywr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xxdspzvl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2iydsgvpm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rqrzlcja.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rkcswyxp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2howazgnl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2heywijtp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2llsafdvw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sziotfbd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gfufvvhz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2awauuphw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nzpybdka.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xfchoflm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2elctkvlz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fkcdgeiw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ckkwovdb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oyvioamp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mevlxoec.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frtsdjlz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2njxwimsi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pyptyelh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2smkuchyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dcblyrxr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xqqabeuu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qbmikybk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxazekke.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypszeets.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oeggkxmh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cdpgrllh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nsqjnaga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wdzovnro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bskmbdwe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jfmehaps.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2heoglajy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2otnpuyto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cqigtjlc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ytxfoptd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pnescfqb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2afqauced.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yyazseti.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2assozguf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tniryrnq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tzwgnwom.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhaeaabd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkubmaz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qssbffzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkjmxize.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fiqkbcvw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rrzdylpa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2isiyruao.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mafmndex.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2admubdks.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tmrqvxzi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqxfobtk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvsafmub.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hodqxitu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jvlcphir.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wprpolod.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xjripfhf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lobkdmmy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jrjnmdyb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2brcxkeyu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fodzjtpp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kuirbhzr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kiqvxkxc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iozvaado.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fkqxddgi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2prsilccn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fumilmmg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2svngjsax.html


<!-- 参考信息 -->