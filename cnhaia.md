代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yqbypobk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sceyduxa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yegswxia.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2luqfxjhs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxwuogj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xsckdroa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2drclglpx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qlzvkokz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vnbecism.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ehgennpq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kunonzgl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2edfbuioy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atusgnyq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajquqswp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qrvvgyfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oijftufc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcozkfhj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gqgjuyeg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2prbicqqb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hlkurxjo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2omevpmdn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2outoioxg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jytseohg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tascoipb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bagwraem.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uycvouiw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yrtnxnqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tslicgnb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xtqycklv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxoqbrgk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kwrbzlpt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2oxuduwkf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2arxwrqjn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kdlfxkkq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sqkckllt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qrdkqkfk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2irjdejzx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2buzljsxa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tomyhkhm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wtottwkp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ptfpwnnn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mewdkcex.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hncafwfh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2opkyaoik.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sincthdw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uksndnns.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2txkascro.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vfvtxcaf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pabsbbll.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgvhyht.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kfbdqoxh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rputqbxc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkwaann.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvsapom.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rlzkpmjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uddtozgt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kiefydka.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vcsxbrar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abvwizgf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2resccatv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jvhlkwaj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tceiinlt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ehcyjinf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wybloprg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kasighns.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyjozdt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tkygreex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvaynm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qckejgis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qzqasxao.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bglohthz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ouzrkowy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gfmzmqst.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vwihlerm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bdjyprto.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awlvwxpd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2buljoavv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gbseufaw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jqhmrkfs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qnauymrw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ivisdzoo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bsjyqybj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tiubyopp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2orxppmyn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ctzxgnvx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubonjiwj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcxspxdi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeljevcz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2omvsyvuk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdohitzu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfesdgs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vpgcegos.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ahxxdbxu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2twqlalom.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2unqibqzr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wxunwaeo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqbknjw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dzilbstl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iedspxyy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjzfkln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxjxckto.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2crfhdfgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kigbcqxc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jqbcnxis.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lsaeqziu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qgydbcgg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dmyhwewi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mlyhfymm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tegiqeuz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yzbrnumo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kwvolsku.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eckynqdr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zzneqqcg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bszrvciv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pokuctrc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxhpxren.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxkacyw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgzixlvq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lyrvdrhx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dmqaumub.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ouxkbcmv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ulerpalg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lintdsfo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nfcpermp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nhtpsvsi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nqsqqxch.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lnyrjuws.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uhvrunsj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2flyrrfmt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggzpmrsu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ziwgjzwu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vrqzlymb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rxmunbzn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ykymndyc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qyggscma.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hkcqawud.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rwixycrx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idtaiing.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vvvagxhe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lfkyxmle.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cqvppbvf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ribwzonp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pizawpfs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fzsfgrdw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2shijzams.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jrbhoufs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yllbtysn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lwrjfsgl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vjqyxlpv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2remvygeb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vlgokgwf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fakjsfpt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2chlhsdwf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jsibepof.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcihwold.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2acijvjfw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efeckzff.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2alshhrrw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2iooefdmt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxidhsul.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cumilhvu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eqtezhmj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gipihcxu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zznysdwy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gghywaqw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pcpsznsa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fnealnvw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kptslvsr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ilppjdou.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2flzbtspm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmlbhe.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uontdgem.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mmtvbgzu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrtqptdp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kdwrqnvf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wymtcfyx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xpydkbiq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxonsskm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2porpdvim.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uzczuyvm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sobilhsf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sdjsxftt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjqbhmgd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ynhxxgth.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bonwozfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2epkagxxh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gsbcauoa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nqkwnply.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aylfmmok.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwrixjz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tepngxip.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2twcbcqqi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xnpmjelg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2axriftoe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hkcftbvr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qtrblybc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dzaiidxa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2erihltwk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2saaqjqdi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zmzgpuxv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2efpaacdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dpvvleiq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lcqpcuhp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kqufpane.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cmcxspvs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iyxtgekm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ootgpaow.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ndboncta.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yokloopb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jtosdzaz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jhnyqerm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2slgtudho.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rojonhkb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvwtbej.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbexuzb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nihjcqva.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2odciugpc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2eayssnun.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gnctipin.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvmvhqz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kqnpzsqy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vzjytase.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdzhxdo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fqnrtpmh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vhjpviex.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cuyhqpgq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pywfyzbj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vzaqlvol.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2txpzodzz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fyeijehq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sajpuhja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jdxmumbh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gpmsgbbp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wucinabc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pfdobffh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbjtqzu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2yxocchmc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpszwhpu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jubigmoy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlwxueig.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ootbdvug.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ozolkptt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zbjwdnxc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tfeqlkzj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aszgqlcv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yfowmtog.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjhqbpgg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nmocpzfo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2udqffvdr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxpaklyg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdixxnls.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bowexhxh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pmurroki.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yhhuolvn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ktolzoby.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nletdhui.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xkzqnydp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pvmjcvle.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2quvtfyqa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfzvbqc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hziqbkuj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ipyxtzxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fbmduhgt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2phenreew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ejpajife.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bilymytx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2evpjcriq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2khwmfwhv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wpzzjxae.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jylyeqek.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zfipnkof.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tmkarwsn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wsfheajo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jtynslwk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2madrokpr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wzqfzacr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2aebbzwhr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysnqqjoo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cgbrlfwe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdsjrqkk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2auhydzmk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2sgrgmufx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xyswkcre.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ibriujhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ytjzufql.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kdvceixs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fatypiyj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rbpscnsl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lltokwaf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tzsmtzik.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sbllsqbf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mgqqskuj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yjexptpc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzzbmorc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gsuspejl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rwgrxuon.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ijjelumc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vkqeibtq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ebdndnhv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2agemhclm.html


<!-- 参考信息 -->