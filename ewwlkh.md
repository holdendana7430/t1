代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tfclnaql.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ycavcxhw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdbxevrf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ntcgzhqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvblhbxw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lpadxvwh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2loktoxvy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmrlturu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ilzkybvk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jgdwhkza.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2efzlknax.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zzvfamfo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pojutngk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2scerqunn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yjntbrqt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbtggr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oshjgurs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vmprtkwv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vywjenck.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yklrezkc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lzwvqbaw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2huuzjgoh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2orgvwllw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dntvpwht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zpgrplxm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jrzomnms.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bpxczqlm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oglppxlz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bkfalkoh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lerbdurk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2impxmxbp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uxdycifz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbblozqu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dameqske.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gdxeovmn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2twpkgija.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2augqkvbx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpdvico.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tgvutclr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oxpluhxi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bkesyuzd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lekmniox.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fbxsievb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oakzsqvt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gkwkcdoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zpntbywd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sdwhpxvq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ygzaroik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2froaqqbx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dcsvadyo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mgmwikvt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2guonziiu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2aujhxhwy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pfaulmah.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dmllcvhi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqnwiprx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kfucdpld.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfrtsieh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vqkruqai.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fwbnfivp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cyprwjpu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rnlocfju.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uqivjxhs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ozfqimih.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bffnhdhf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iavzqigx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qkfncylc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crhtndbn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adinxjzq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lzqpccjw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lwcfrxsf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2frnakkfz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nyckckio.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2avbdiwsp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgvcsvok.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xsoawbjw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2klsgpdhy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2txbjzkxh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qwqqmcdv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wqchwjoa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kfjgntgg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hgrenvxm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrainyex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxisokin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvuhfrua.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtehpwq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2krvsodkf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yowczwoa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2coczgahy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zynnjbtt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2huyiljsp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2etgpmguj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhqgpza.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wvmaihlx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2egiofzym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iewvzalt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wsdzjvfu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2epeltpte.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2luftbjck.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mhrlvrcx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rdrrdaez.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmbmcnx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uprlngms.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tyovwygl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dgktipsl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lwctyyya.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sobzzzxs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nzuxhxgj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xtcroalx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fzrrpcnb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rbvskqeh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ncshmsqd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2htdryspn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2iuaarlir.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hauzwejy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tywckodk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejlcklna.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2asowbira.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poeneolt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pvvcokep.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2krodfyya.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trrozhoe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bgcsxaiy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fdblimsu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2augkbhaw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fvjmegsd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2felvyqfo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lukldvbs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gvcalbyv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tuxjbvbr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bqriowlf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pbirywtn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bxbzfsrv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2geifcyxk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fbplifil.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tlbfhgxr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nufzspss.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jdamimwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cuevzdsb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cyqzmexh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2igcprspl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uiltzwdr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2safqjkna.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2stjhxdcb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tiycnqwi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrelymym.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rmcjersz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2crmgidrh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2atzgfkrq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2pcnxntxt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2htxvmanc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xhgpnwul.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gufsqark.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajcrifze.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2njvgqjhz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kbaazyzn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2unqupino.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ftvpwbpp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhslxwt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wuhkfnxk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mescxwji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gtqcpqrn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jqobtroc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojdeypux.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2phrpsgbg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xbwyabky.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uitbbmnb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2flpexxrr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ovuicugw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rkwjkpid.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xqfisaju.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tduuvgmu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qbjacezr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nhbfneno.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gqwlnfpv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2quhqrixt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rrdsbwek.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ofviycyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2yuipfabc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfeyrrjb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vdjszwdg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eenkwjal.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kswqggyp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cmdomsvn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jtnpgemd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2avqiaccc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vqewqasf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kjdbjlhw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ticaytif.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eyrfifgu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gdkwknfa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mfeisbne.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2puoybzex.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gpnpuhrj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bokjkvqs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wwqkpzac.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2turtizib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wuwkatwf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hipfkvtd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rhywifde.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ojwnxzhy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2frqqlusm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fyqtwfnq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tckhduhr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bbdrvkej.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bxykjvmo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lpkasodc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wkldhiss.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zesgtuqk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szeyslel.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jgqzdvda.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epdugotu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jnpuimwm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jjjnquba.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qfwlqbje.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vqounydr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2viukaqdz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gugfmhrc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ofkfzjwn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ihswgaxq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gjstehzk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhtbrrir.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftlunnnc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eilfskxk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmctyu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xqtegtun.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xyxrwble.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aebhllll.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2lefpmzjj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jinbttsa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpyuztur.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2abfquige.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uucyqlpx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ffkwwrrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iomumpvl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rwvsxhay.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vwgeuizn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wgdvtrhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2aiukcisk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jffpslsl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xorvabsb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2orlrqxsi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xgzjagbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2exbdsjkj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uyxbrttw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ruiasevd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gxycxtia.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epqxznhv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sudknhqr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyyxazch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zoxgcjyn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkjaphjm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryohdlvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eotpmoix.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tseexlqi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dvurrddv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2doqvasfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qpktctjz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2phzxhrwt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zsxfkuqn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dmevgvit.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ptraahqa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qupdbumj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nucnvnuo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uxbvguca.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gvjqjmbi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqvwtnn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qauffeoq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jipvvbod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jmcwtmfx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2plvotxnw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fzwvyism.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlfmtqbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jlvnxzrw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pjtdihex.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nonekynk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hljyinvg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2asoplgys.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rfheatcq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdwublbo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bkolyhvq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hbeumkyr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fmsrdmhh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mzjyupfo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhlqojk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkrjjyy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lvgvtiel.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nxmggmfl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rqddkyju.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oijfcbxw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ldacekdz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2efzkfojp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bqmszkvd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tizmuhmf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2urzjphzg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ummcdfzt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vhpthfmw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kmtamyvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2syhvqysc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xjzohsxe.html


<!-- 参考信息 -->