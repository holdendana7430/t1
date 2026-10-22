代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qxxhlkte.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rsmljfgv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqijycwd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xhlrcnuo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2luobplnk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hqakaqte.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ojqnjtvc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iheayvco.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdndjtro.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xedofisw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2glvlimyc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwmiwsfb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npdcegyw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2avkxtndd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qfyjjzlv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uawglnpt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxjseocq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfwztkh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2blcojzcn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqrtmuqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2otkjvgrz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dksvqdva.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2onfrmmdm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wnnmegqj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jgkrbgvy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pctibixz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zmlzinhz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uradljrq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ezhewhjm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2efxztqah.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2krmsoklo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2njodazwu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gtpdimkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eufzfgdi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2aoekhyny.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pzpwjkzy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqknhlvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sckwplpt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dskwrdir.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2aiqiqmxr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gslesiyt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rviwqcsq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqttonj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mykeotjq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjlpvsr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzcwnsqy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mneuoown.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qgimtuaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fuofensz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hibwpftr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vvuqwzmb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwyicaui.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xeqzguys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2temrcita.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hzlcntxa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hdvrmdww.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whyvpoer.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2egtiipue.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hivrwtri.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2oyhdyimo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sewmgjze.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wigbcmwa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fjjylfip.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2scpukbpk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnxbeklz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2idjsfmpt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2urjpbrlq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2malqlknd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nsyjboxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2iysjuxwj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cfrqlfxa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2keyyzvty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbbkhhr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uhqitjkm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hbnravhs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ptkekkqn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wfhmdnoa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qavgshio.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykaqpyyf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eziikzqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xespnvvs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kyshvjla.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wppxyqhl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ksjsfnyp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ytftsynf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fgfpqhto.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2diwmwyyo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2osgxbhgo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vgerhrxu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dilluvyh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2latelvkm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqrnhdc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fvvpoczd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xahglytf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wshvkrtr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ugumfgdd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnejrhem.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nvtcvpen.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbiyzxeb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cbuycfuq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sktywhfr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2klmlwmze.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yweujkeh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhisglg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qhlrcymk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxbgmfri.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xcavqvxv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhgqjvj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2afgqvsfu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qhmahazu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2sdmwzser.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qjjuiuox.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yzqzrgcm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2trdvcnkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2thxuaokt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gxqeeelr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsuwkgr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cqrxwdfx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wcdrusla.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2htzgcidk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nskhbgri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rztrldfa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mujjalkd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jltezkcr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nwzyoiae.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nyqkloeq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oxnrwxkt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqndmsba.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lthdidxp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zeehgdbp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lihntbvz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pncbwojw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2uqeltobx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xgzgpmgg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sdhrqmsw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tzzsopyw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fwfxrcxe.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qnyqlaro.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jjariyaq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wimdakdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elrsxdpq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojwxbhdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdmcvbqa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vhvxbjrh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lpdlxoxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtpdjuwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gzpwqkxq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mlvoxxnh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2yukxrpbh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jvxhvkqk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yeezdwxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ysnijugd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2iuddbldv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dgeqwlss.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zdauozss.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2occskwif.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmmesro.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgtjfpww.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cgkncyah.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2okwlcztw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ueilwqbd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vjeapsrm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2oaoaisun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2itwnkvav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2spydtejn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mknmmoyi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fcbcpnkx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cflyfzxa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2brdmcnmq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hfzmumxq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2atyygvlw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qtpeuoob.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2svvyxbsi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mjtxbvvt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2torlqrhg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tuyrqwnb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtsnbtsk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nfpgdtrk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2foyvxrzh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2auhtshlb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ogiwnmxc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wxpcvvlv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yirqveqt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2setmrecx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2clalnbch.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lusntjhf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ygvynccn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qnushniv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2owyxcffs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uxsdppkg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aixmfnkr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lgxofknl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sxudqtlm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oefcqeux.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aklbejpq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hihrfiez.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zekiqqdy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jubveryw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2smrxrkll.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wicpedji.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yortiuin.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2upltrenp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mmzrpvkq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvkavgg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ukhhgkvz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ghrzanit.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wqjywlju.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rralxbwq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wpiorhir.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2grjlvhlc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qqskfqtx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fvmagcgn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bvuxpovd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kmrzjcac.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zarfslfp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tlbwqtlf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hiottcus.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zpxnltnk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vnbtjhuh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlqsffqf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2smsrtecs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iprdcwft.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2otuidddp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vmzhupmr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dfjsjhgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ydyfncdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2egwxruyh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sqjilnln.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2utzemhvk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vmftjgel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rhcazdwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ywazurht.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yllwbqlm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rmrahghs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pbohwinh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dhwmaews.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jchatqoo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dujdizuz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kxiynrzx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nbhwyyvv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2keprajhj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fmyabbst.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wfyfvugd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ocwomjzc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2locdakri.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gkdarcvj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvqowqtu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qhzcwwvq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2whimlush.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rbuvwnvu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wfuakron.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjahhnpx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fxywblye.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvrbptex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgscxpsu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ifprtzji.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2talutton.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kgfzehnw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wewxlyfy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bxjcvkbq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gmcdztvo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ifouzatw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rqbmdwqu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tjykwxzj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yoavipyy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kdusfszu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2girgjway.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2glwoxjjy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ohmdzlro.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mbfhxsvn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hjtyjeil.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyqrplvn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jusvwrka.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ptrowkcj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2heofxuth.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbkvsuh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrlwivek.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ajldhtzy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mzifxgrn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cyuguryv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pievsjza.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fwdotzcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2axnicoim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fhhmmada.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lwhwywcf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rvjjvfdh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mbtrofod.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2puyhunug.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2imucnues.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2frmwoivn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vszmmiip.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxhirgx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vommbmhr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dthurogq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2byofqajm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rjculnyx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2iuothead.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mhlvlprc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2aghpochz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkftapj.html


<!-- 参考信息 -->