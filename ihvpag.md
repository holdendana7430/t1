代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pnkmwplt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nzglghsf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ghldnvvm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gfgkfygg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rlyjakjc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jcmhtkex.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ctjkovcd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zbhblral.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lorzxplx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ekzapcls.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wppkkeqt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xprmelwm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3plnwgmir.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fikcessq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gfamphic.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pcyohzyz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ejmadlez.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gwnqvort.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3biqisdya.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvqzavqk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcopinxr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fsfexfwb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3woehqugi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3abklywzx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iluyfvrd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3exrcovif.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jecnvydq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fciqpdii.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lfwxxumf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3midbezoa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mxddcfuw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jibwapyi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ngnsbnzm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhtdugri.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ztmxunvy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3crkcgqgf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tobioalv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kiwnespr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gvmshsix.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qouugbyc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nxlveuzr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kicvkgyp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cugrqbnt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vohgxbae.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xyhqvpry.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tanfhkig.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axlbbvbz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ogspigge.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vfdbanap.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bljpxupm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cmsoqgjd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jqrvlwbl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hgikxpct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wotzolqc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qeqqmcpi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rtgllfwq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mkwnisih.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbfzdvlm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmsdvxmo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sggdqqnv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twyslbxc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3petjlddl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3taxklthg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3sqrohtrh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqxoffd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ynhsyrzj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqdoortm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kgmfmwqk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rulhqgan.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vdkuwtzk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lsvsntxp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wnqwbqsc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3opiuutos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnuawfkz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ukpnesya.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3auaoqxto.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzxespit.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wzzkcauu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bnhefqom.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pbhxyemr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxqzzhv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3seqegqkk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ansnwwvx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qqrwjlve.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxtwrnr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zzvpwzvv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fcomvola.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mtzziwue.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kfzhxzyi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3eamvbfgv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dpsfqfmi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3skypmyfm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fcbpkdnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3raxwbifw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bgcoqnsw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtuvmnya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gswdiyry.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3poaqodrr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3abmopaak.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fyoqtfiv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jvfsireu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rutdnsqy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yjydkadl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fmdtixlz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhcqhdpv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xfzdrkzr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yzmtqcap.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ixyreccw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqstywjo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nizyciim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjzsndfv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gzhtjegr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fsipjhes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cbeqoqhg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xonnykmn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dkgteehp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hcmcnlmr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lzsagcbs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ilizbudm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjooimau.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mvahqaam.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tmykmuuq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3avfgznvp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcyglfo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iholyohg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rbevhymt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xhlztruf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uyfxuyqs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rmmgibkj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lfgpavhu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhellxmi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yljistzp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgsyzz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjlewgh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmhmwfv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3khqomana.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3snwoknyk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3aucxgknz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nmdlvjtp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fxzeocjc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dtzdigfd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3snvcarrh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jwzqapjl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sjuywzst.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bpouudlw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kpmuuktq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gopzendh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3iauzoimf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bgsiifbr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dqvaflaq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3havtuvts.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ikittcog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vogczfzx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sbkpnajd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kzwwrwrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3svpogxgh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jkzrcwbv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajbmqdgy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihblhuiy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3shylpxam.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyqtyutt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdgpmgs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndqalkmu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rlhvvgpm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3novdhgvu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3agjfetyt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ladlmtms.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyarmskt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ebzkyriv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vaojvruf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qtkzrhgh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjadkhv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3mddaoxlf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhicsq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zdjtbeoy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gjxgrmsz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3osfacriu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvnlwz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3paouisgs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nhjhscle.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3squbqeec.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zfcnwtza.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ilaourry.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3idkufexq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xpgsauny.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3saukjqpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mhhfdmft.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jtvcjmfu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ohegdlav.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qdhfwxpw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iarvhrwh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lprpxctn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cjdylktz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yxjovudd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rotluxxz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3irihmloa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fxxzkrnk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fttcsuvl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dbjqwovq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uapbcchj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3atzvanwz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rwhrqorp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3owzcjsyw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sebgccmn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jkimlrcy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgbcgvkm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ipuohteg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fyrsigzs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qhthneqv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dgbopszm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jptwzbqi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xjgsbfgh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xdtoqfqk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yszyaprc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ypaugyqg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bnhhqygg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3utrdmolq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3govqcbtj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yyjhncmr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nisbcqhl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3arbzrtak.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3waipkggr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvalotzj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iingmpcz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3serjlpvi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3npehegki.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xabrytlf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvithnsn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xfooumkb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xwfeoesr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbgqjoyh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3anfaogsp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rcgoufxl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ptdrhllm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eusltfux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sjofgmbk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qulsuvcc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3snfgkevz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3epualtla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sygqptsw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bumrqhgu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cvyvuldh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3znybsfmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxzadqqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbavcyx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpfseob.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bobkcpfn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dzofazbg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rqkkriyw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pfsoodhm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uiggpray.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ocbhdelf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vtzkolck.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yuyqvend.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3pxyngfep.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zmztfkgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3terxwdwi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppprtnie.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3smadwpwx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qceyvdsh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ucckleij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kahsxlaz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aanoodui.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iobfxxyi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vkauipwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yduaauql.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oqctzgoh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbqpvxl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3abbvsnyz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3loenznuy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vogaymgn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujzzhmtl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3thwrffnw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yzcfoltb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3alaqirdh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qsmqlhsm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ashekzms.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rptpkngl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cnoxslzx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vdsxfeoa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ygevaaxq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3peohzbge.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xzmzwhhu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rlkujmxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3aswaiypr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3poijaavl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlyyzvys.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dscklqcg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3psxkqeeq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bgvpucii.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epffdmpc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wxtjjfrw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3afomrgwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mrisqlkg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jjkofrwf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3epnjdfuq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fafarmkd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jwfserue.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fbmxyomp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wgxpwduh.html


<!-- 参考信息 -->