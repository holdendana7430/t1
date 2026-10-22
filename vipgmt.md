代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ltwcpnol.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wyitulxa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pziabujj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcyvqvi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wqmygtgi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejepxjgv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qwqwfohr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lgmgakvi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2raxxuxiq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jfoywzup.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fzcejiyo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wysspznd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mbkssnkx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfyqxylt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2offuvmxb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpjuamqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mhabvbcm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2yzuqbzpz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2seeqjqhs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zrpzutpw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jthlwipz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aozvcvfw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvkhcpo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2weoelvrl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvbhhhlk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdffpdam.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2urdpnqpq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xbffyxbq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ejwawuas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dwpiltid.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrjzymgs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2alklxngu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2solbivtl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dptyeyld.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jzgzbmiv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2whpzfvjg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkklajzo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nsdcdndv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnfkijfy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tjjxnexr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2buvwbwhr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ziotllnf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2caoyvzyq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zvliodza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ikwkvehv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2eegcvnyl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jujnpwgz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwoqnqwe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygdldngu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xelwyssg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rimwwoyk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sycsocgl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vfpnrrgo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uiejvwfd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ujxtzrju.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zxavgpqu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yzwpzzzm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2annmoimr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gwnuxxer.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2soldieye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mirkwovx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hslorput.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wrkyxbwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ecwubbef.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hkprdcip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uzpxlclb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ysbdlgmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2grvwgemq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2reodmfmt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xltotdxm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pqxfpuqz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rarjmqph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2anfsjckn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wssqsynf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnnrtpuv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bacubnxk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bbzxprto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sggemlmr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lxtotgil.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wgfokfuv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fwbmlqdi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ofxzuayp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sjkynusr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fchzadke.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hphfjbjj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2amiypean.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fsqfmaqi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivpelbes.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rdndiwyw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ujcmddap.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwqdegk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2thultfvl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bklyfvhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xvftzrty.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cqcglzzx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ucprkcxg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dwjpemnv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqbqueo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dborcqwj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yvgyvlsi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2aotusofy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rflxcikk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cofbspyr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwtcjdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qctfunhu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnhsgwj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hmevevnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fwhruipk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjolwcxg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tgyjwlbx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2htinrdga.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcfnbxho.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2amsneskm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xduesbmd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2okzwigib.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tulsdfwt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ecnfrcsf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uhqfmtyg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rsuefwhr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vwwxlaee.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zpljxdqi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnwewqg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2aczfyvdb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pejcpnez.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pdhwbzlv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fvogbogy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdvlcrp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpficzyn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vpphkgbq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzrzyhpk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uxuzzkxd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uearngtk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wqfgqgun.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jykgrurj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tckgejpo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vxiofsyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gexpwufh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mrhoqiof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzupfesn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vjstmbdo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2egasdrsz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yxidvtri.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2oexfmylx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ejmiuzgl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zimffuuf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2muphabmy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2blxybvbl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ehpvviax.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcgqjqqx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ehtphwwl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nbjryfod.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvlhcqqc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fgaazvzq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2prvibrue.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ujaesqqe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2daprotam.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2manmrxqr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fuuigcws.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lzpjvwnh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2djlmbdix.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gmdjtevq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kznnpexk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wokipnkl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zwtcnezy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vllvhcbx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ielvoase.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zqrvmkkt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kqkxxaxs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ykvuawiq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vdevrueq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mrzzfals.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ltaomgsc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2npnxcpci.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsjbajd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnjkxsa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lvoygwxp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mccqacrs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gsxeltbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyyzdxrw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zogvvgux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2apvkiako.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2frlckccq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nedjnvqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qvuipuns.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fpkzmvss.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gcctwiha.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2edzbmdpx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbeahy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tnnjndjx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hrburhyn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xfdrgiqk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpujlsdm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2doeseock.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gxadqdrr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jxybrbol.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rzzgxurl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjigtgzz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rkxwllju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vmupmsbe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mjzziekr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2apfwawwy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pjjgxfwm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rqvrygjm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gmopjyjh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gkgydqsu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ttvwosmo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ygnkikei.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2weojpipf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2exjhdbcg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2itpubzqv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lqvbwgfp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2semycjph.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2quqzscmr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gdxztswm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rjewgtrv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dvarbyms.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qgevnsvp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uxplrvoo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqblofc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vlgkilwb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hdplimxd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbgvkr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2egfvmdwy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pqvloltw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ikzxvmst.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lelufpjm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bkcrbvup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qzxzucvl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gefuuaua.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bodqxtpu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kklenzhd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbhozefe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mnwyxumj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dzjbpmyx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kswaswaw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eyoqkenx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hbavcsgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hxhwzwnh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gpymugwd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xkxvkhht.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eripgqvr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ironilzc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vbknrxkh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ksjstuyd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2liomqcbk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wxerxdqj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ffoszgok.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2weykgdzn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uxwcjcxo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vujlinrs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ospfpxnf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnrxjeiv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nswqogbt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urrgevcv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hpumzxgo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2txbuyxif.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2frfbgijl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ahhnlwqn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ueipjpri.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ilenvfpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2igeazsed.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2evnmhiym.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mureliak.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2alxspiiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ssecdzfs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2avbjhiok.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxudmwu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fozgodmy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tdcenhvk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jehlfoth.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2thzfuibu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ypjbwfxk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ctvbchph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqcxoeh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zpmgfadr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2guyotcgz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2plcpvzkx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2afottbrb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2edixwgru.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hmfbzqxd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vrbrldka.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ekuxxrpe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fzryhdjt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2umsjbvvb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bgpbgtnk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecgeqnhr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkcnibnp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwqqoif.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxdiglo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yogzlmeg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzeeit.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aopoctlz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2oszwdmqj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sflwmqux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2oquxdrjt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gfwhndpq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pamfhgwm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uwkennpy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qyycudfs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jikcvpkw.html


<!-- 参考信息 -->