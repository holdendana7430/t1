代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2topyxzfs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kbqggwem.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mbhzctcv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2waqubtna.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hokpraof.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gsrjwauw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xfovlkiu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdqykdhs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2usendoos.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jfeqnvuk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cykiztqp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qibiymcg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bwsfwoar.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwjqusar.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzuwyqte.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnfomng.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztjsokns.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kgronjkm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2srmfueve.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2skkpmbis.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xcyyjpyd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vbbpxipn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pfrubobr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tgpcouvl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gzphwdbl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2clmgtdol.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pawifogu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bebyyabz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpnglekp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fxzsteqm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2suolqznk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtywftec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vgljmsak.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pjevsnnn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xixxcysl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2pvehuwgp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iyeesxxv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hdehglfc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2daikkupd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwtovcst.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dqzprmru.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wukizzhr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nkavullm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bbmcphoj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mokjfwqd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ldacjvri.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zusnrylw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2liwcmcnk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fhnbengh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2spakzexx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dnwiaslx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2srlluhzx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bbodspuf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nwcpmzmk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sourhpyn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpptcozt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fikvyyun.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aofulbkt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rbpkjzoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wwgjbdfu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bkergnkm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lzuxgxeq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jbbplfbs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgjncx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zfuzczam.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hbvymnya.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zerouohb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2grtdtdig.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vwkjunom.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nvucnomy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ullxgrhd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nmfmtwqg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2agelfsto.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rphbraoo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vxhwjdlp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mcfadxpp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tsjxvxsv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2multuohy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qxkdbocm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eqnwbteq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uczqjket.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmntlqby.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfhftmo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fyjlsxhs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2afydhzae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hbsctubw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfelhyce.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tcfwtrjn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uyklqfcv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mnfguknm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wrhxjthe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xmnhcpgr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wipnuvgw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ybxmpvwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srbblylk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kysthpdn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2judecryx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oabonrld.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2erimfzkg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pdxfjdhb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vqjgqdxe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pdwtcnzl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bcruizyk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nzofbkpc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bkyosnpm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lyjjrnyn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kfnjhnuw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cihhintx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjdwgoj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qgoqfjsu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fkhmlesj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kinygjbw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qjogmypy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhnreqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cxmqycbc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cxexylgj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2asueltrv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eocpxjik.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clzdrodm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlvowxwk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fwyjkyak.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2amyuepfr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zqdnrwpn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2miynzjiy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsldgau.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zgcabeki.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tftsfzdp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ztlzbvnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqipmhoa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kzqoxapb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybedaftz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aivrcrgn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kvsomfwx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yqnymwaw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sasqdzqw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fsprwasy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2prwfjwbc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pbpgbote.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ymnbwzkr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cnsvexcu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osxxjhhc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vtuozhwn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nqmahmmr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxuiqdvd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ybjxhmfu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2waoiwsrr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2elnxbkdg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2euurzbst.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dgdenxmj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2srlrlzsp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yetbdpwz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gfgjifso.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2isqzmbsx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nhztwotv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fxeohqtn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ipechakn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mbnjfule.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fidoirqp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bjdsbjdp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rzjwyqfb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xvouwnme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vokeddee.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfvtllxh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2diivzdzr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sebcmkvr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vkeunomz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eykdzftq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fuhrwzlr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hvrqdqhc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2intnlhdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wtdokcoj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fbinumxi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zlknesiq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xoltnxhu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2djbwmppr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnptwzrf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jucocdzm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qhcfldho.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2efrevztm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jupjytma.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgbmjrba.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxlojfww.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgjdkzy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gxeojhsb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zaouodbr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2npftkdze.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hmgfinxy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgouxia.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vbmwryrk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sbsrchmj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tacnroax.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ltmspfhs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2itudpuua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sfrwbkfn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vfitzeou.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nsbrxtiw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tumsowoe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ftvgugct.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gvqabhwp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2plrjthgu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tdfmhcwp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwkwwjyv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtmfelj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nnpkosqr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mswkecbm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2abyhvyzn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cealijmk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qvwhkxya.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jlczmusb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vqoacgoc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2iqzhjdmx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gpmgncam.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dptdytyg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mwiveptn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2estslxog.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lefnsvuj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rdveswxy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hadpghrc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nfivdelx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iyohbmew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2imqmwrmn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpfpmlxx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xhyyaghg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hylbditp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2duranoxc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wigufxog.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2llljjmxq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hgubmsmq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pyaoqxst.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nekkoowy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ledgegbm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmoknfrx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2upyzwugw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2worcjdyk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfoypckj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mzgeaoru.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2txgmvzqi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jawkibgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ikukmnlc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hoibbajj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qroylnjq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2autyigfc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2coatjipx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysowloac.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uegtpjqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nvlwvwvz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2etcpdurb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmxgnlix.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ezkiqhsc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kocgtzaf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jnxelpmg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ryvyqtdo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arkrumni.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xchhrvln.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tyvstoxu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vtlxlmlk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bwterneq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jqtitezk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcsmbuwd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ennogeoj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzwyyjs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tjcyoira.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2efvfsqmc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbuofyv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jseuuclc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wajzcnyo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2djhdprcw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2awtauqjc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gzotjzwf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2serazvqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oebbgrbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqiczqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2emruwfql.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jokyzdik.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxjqrmts.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vvscfhqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qetgphjn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pvdwxenq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpthdyvs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oamtvbmk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owbmnpxu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gvqdtvlu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2agsbssax.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mpqaptvd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ulszctwr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2aafkzrpl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ekhxrqwh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kvwvnjwq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvjodudo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ayjipqja.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dxdidtdf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkakvmjm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vzqlabaa.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hgdpqfes.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qcrwxnia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dgbxvpbh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vppkxmag.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2itielxdz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uktdbiof.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pdsytejl.html


<!-- 参考信息 -->