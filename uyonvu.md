代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fifmssjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nnxdhbfz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzithju.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fsjatwab.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2itnwucur.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dnzfvdux.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xulxpeyt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qtndxcvt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fgbjsyhe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vwufesoj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wauyambn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ojndnbmf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fgvbutvm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yiazjgyk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xocgooeo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2phiqiond.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zslixvcn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ubhrkaee.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uiomywkw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sofagcst.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hwkwcxte.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hjgryxyn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cmldfftr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llyddihv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rfheiltb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nhyowaag.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yyxrxpin.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gbqxhvvb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqhkhjm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ikiuhqyi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qdldnnkd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iuvrgyig.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jdpdvgiu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dgwnasxn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qotxwkis.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pixvkpuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jsbotzzm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nzzoaasq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zwkumukx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lyfwggxx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qfijyfcp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wwtveuop.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kjsstinq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dlfsmxxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2syvszado.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wuebpmdy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uafinidm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2beazerzj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ewkitvay.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mcscrmdd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wetjqntw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wlrmsvsc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dolvxtfj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rudxkykp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pqexznbu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nviufgig.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cxvygbjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ignlwjfk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vunfqtyi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dcgqoguo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fihvogqk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2apicbyak.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvyhwste.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpstnjry.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lsgtxgzd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gofpxqro.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xszeyxwn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dxvwtnao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjcoikl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vmnboeea.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2odlixyot.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ducbhjss.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mdavrhru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjfuusz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xgwzcely.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fagkjydx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rkslqldg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuxcgtf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bfcdybzc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ilyfowmz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fyiomzen.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qwmblpnj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2prpflqhv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xyksnajb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejiumlbd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ddmeconz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2cnbbgyap.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2agogshkt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cekpktdx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvnwgtpv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fmwihwlt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2iwntpytz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rcarmfkc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2usqjfqaf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2aqualebn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tketkwhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cuxywqdz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xjmvyzms.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmpigo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmrnpfy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bwqanbwp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkudptmf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2grdlzwva.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2atrblitk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lkxjukbu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2agjpmpvv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sptlexbc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddnhpnzb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2icednuhk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tcqxjhrw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cifsdklq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ykgtqyix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bewiumsy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kndejpzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crsuogab.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2upfbxaiq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wvqhebig.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rpmkrkjd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vuzzbmbg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ihqcfjdx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dcqoswro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mcrhalwn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bgjkocvi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mimsfkso.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ftzbultp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wqoqkedy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2teuimitu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2knbiiuag.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2grhriioo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2urtonluq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxdiswh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pjsytjgr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lwfgxppo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sslmibsa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vhbhbkcj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qonaxsgo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wwjehent.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ulizrmwk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xviqsual.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iqypgwwb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dksceqcy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jawioowq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rwbzmisd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xddufkff.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cegrqdid.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ojlyvnqx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ooplcosj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zfhxzkqf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qwhzhcib.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wykyhdpo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hknjomlb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2btkndeqz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zlzflpsg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hdijhpyp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lydkerkq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oyxmojrs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ewjqixtw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mhaetheq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2txhhzxiy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2slfzqayf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hbemunkt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufpfigqv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hhbgeobs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gpnnowku.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgctmnrj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xzdoigaj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhjknfq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2igguoaqt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wtlfxuqw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ijrbqidy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lbkqbwxc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uivtipea.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gxuwlcgp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ovuwyakq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cxoihbju.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzpnmqhv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hgiljgaz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kpgtmspx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ulzbacfl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ngixpebe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2eurndidf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ylpxtnzv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vedtelee.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjanwiq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cotujgnk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mjmvvclg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qaevwyfa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2swshffzf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aextbaft.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxywcmep.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ndynqikv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gnejtaul.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2snopryqz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bdoicogr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2daftvqiz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozjuuxlx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mxpltmpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omtjwetw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lvlgjdaj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pkzieotm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgbtnoo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pauhfclv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rxqyvwdd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sykghium.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hzsdkzny.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kbxbuvnp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rnmrjggn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awqmtpax.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqkjflfh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tgnxdiop.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gzhscxmy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2atjnnxhi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wvvrmeuo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vsipmtwn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2abyjdjxg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hdnfnysb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ersunewr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ojywrrqm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bomsqfbg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uqrnxgoc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2joidgewy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hmvihrcj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2miocvbkk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gkawtcra.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzabzgp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fllptmjk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qocngsca.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqqhvfls.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mzpywtnj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sifpuudy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2npcuomtj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkbypco.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nvddhdwu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pxrlwnij.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2luupwedv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dophjcae.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znszljmo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xxalwbjl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bbtkkzyi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xtzpediy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fodnmgra.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qjlzathh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aoozxmsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwubpsuv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxuacpxx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hsopxhvz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fmhjaxup.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dloqnyig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2egfjmjko.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ddovznjk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ggjkjaci.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qlkhsxei.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rgvuains.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ubirccvq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2alhqweto.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jbufbsyq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xnuwvety.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fcpwkfkt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nfwylijg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kfqefqkj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qflmhaff.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pzigfdgl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kavdmeek.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dnwvadhc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdtviwa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ssnbivxi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uxqbgvan.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nigybjgd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fxndnetv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2prqsrkvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pcyguhmi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfpalel.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtvpmbli.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oipjfukv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wuhwqlsg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wjuqswgt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ktceurxz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gufkgqxj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mkikcjsn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vljnaapl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eiimftld.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2joafigde.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hvwcaknb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vcwpyybl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rdandurv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qhujirvn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2judgywsc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gucmfudn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fmfvldxh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2txritxhl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiksrnob.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mlrrnoix.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cabmehjn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mwxhlgdt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juhuybav.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdgwhr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fnsjslbx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2thoqhufg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abqzzxoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2chtqfgvz.html


<!-- 参考信息 -->