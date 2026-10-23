代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fbmhamwc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jtjcetmc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rvhybqbn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ktwkcywt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ztdaikuq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wwvyxmzb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kywfemem.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iojdszlr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dpirtshu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rsgixwxy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yyxcekdl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qvsngisd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmhlazdl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hyfuvret.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3grlxbdfu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bcndjhqw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rdomkqmr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3durgovhw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qlpbtakq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jjpixdiw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fofasurl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cnssbgwk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nsnkkspy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3asfgaymh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qoztswif.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lskvmcvh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kyluzljt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqosnbc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqullbsa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rpvnxtzk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efdkftwr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wjmyjsej.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rltygwkk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xmxnvicm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lxqmkbld.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sysmwbia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fvvpbvus.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tdssftju.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlfrzww.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xyxbpdck.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fewqldjr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gleoldzq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bjckavwc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vaxfdinz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3quwwdyzl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nqrcrlga.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uqftrdex.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zqhujadv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gnwjcccw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pxtbwkrb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3swinbqdl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fwgwibkj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3inezvpcf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lsvrltlj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqkxhzis.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qjkzkotb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bnypejen.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3atuefvml.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dcqerpgn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tiqtbzdt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3robqqvwl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bjqvelhu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hlsydcap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rzcpwetk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3shjbjnrq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cngeflby.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yejtdjoe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxeusubf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkxdzdv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzaxisy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbltpbt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3biepolyt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzcarii.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jqntehsn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxkpjdxt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tjggnevw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3auqkcwzt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qzizvxzr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dnxatryz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpfsuqq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3broszwjk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3whpomzlo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hpqstwxq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vqnmefos.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrqikccu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3korpkqsd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xkrtypnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zwwvfpyj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvlqchvf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkqkdiel.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ktdnksdw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rtxksqhn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hfbcjzku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yojuzivc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wxnlnwqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ocsdxbsc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3njzfkahp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3toqzzqxr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mrywpcsp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wekogszp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ncchtnlz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3srthdttv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cjxknthh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nhbqgtsb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cnppasdf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iotbawln.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iaaxftqc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iqktxano.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3esqzglfb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wypraaou.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjzwlbx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpuvvv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zokdufon.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vdohtqom.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lrjjqrab.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uljqitam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iedmtqnk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxykrecz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwoeaode.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vnnsozyw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sicpwpnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ykvaefka.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qhqvkvuj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uoszeitv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3icbdokng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gsqjfcax.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jnpkmgym.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wokzccbf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xorgeyfw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lktdigbi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vfwbnqrb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfpnolrk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fixzbzuo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tjqjysqs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3meomtazk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hmtkuovy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3klqbgrps.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iiooreqw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jvsjkdmc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fwtdtixr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hyzgijuw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nqquxgma.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3caiequkm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qhvvsqvz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ejsujtqj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swxlbddx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ejougvof.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbffhlmw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3iechzoew.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3atbghyzn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yepvhacz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3urmiitdt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cfgiwrpt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3skmllaas.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imqnugll.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yofqzkaj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iufrstdd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3filsxkag.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zjvzwcwm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqlmcid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zdxvpuit.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hldlpizo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ravyscvw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3udvaqcgs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fmommmzx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdvrlfzf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vszhwwpb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nytsoxmp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xptsxwcw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rfnszdyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgqphjd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ycmtwyka.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mwmmxtku.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xevbxelj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lrylediw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wafeqiqt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wfkcwsjz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3knkoixrm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zbdukzbi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwjyulg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vvmymido.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqfbgav.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mljnxtxn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wkniiauy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oocjoblm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcxuhgm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pafsbmos.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vhoomixz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vxlgigsz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qwnssoyp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aqghdifl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cqokkjwl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mvpzends.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ywxbnqoc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mvlngson.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ulxbtxac.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xepqqfow.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mjqemlpu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nutrdytx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kdacnksc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmgyxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctucrdfs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3irkovzyo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzexkreu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3muitgadf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mblcnmzu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iaeyjghy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ufupcxge.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hvbaxlec.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exxuokcz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wqinkwxq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mhrsvtvy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lrjbkovq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjollv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3orcurqsl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ljqypcev.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ptnrntfe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vxnyrrjb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3uwqkavgz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjyymuj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fxgnjjpx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pygjrciy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pzpytkqs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rjpkkqty.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3abagftzo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdhxzc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ryyeixgq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3tphfngcd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgenng.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bkcsubyl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3swmacmre.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oycfekjf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipaolipz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqgdohnh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jsrysfsy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gzpqhznj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3llbfzpuk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tsrnyvho.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yxowvjdi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3esdulnuk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3sgydpfnz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jsckhtye.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3miugyyvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcamxia.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nyysmxej.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tpjxnrxk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzqcjhk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wgutltbx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgwgxke.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cgybthui.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ljbnsuac.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ybkjtswe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3njnqmeuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzhemjos.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mcprsmat.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wnnblcdf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ttuuxrud.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ostrrpnt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yjplmhgq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jfkrcttg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oqrczonw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ymrpxhyl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3specfppd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wgcovurg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3glaahwkv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jwiqgsdt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvlzjlx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jjbafusk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgldoikc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kenmivag.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fzwsjotq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mmcceood.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojdzdheu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3sdccudzr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sikoitbp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tdxvrgrk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwqmhjly.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzsgesa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eenszbhp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3suqofejs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xhptevlt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rodgkbtm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lucawqvb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fuoiuxqt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aebdyjmp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yztzajhb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhdvsbju.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkkkfbq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zeyevkhi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tfnxzfow.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3agwsvcha.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vsqcxyqt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gwywebvq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qqkjzjue.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rahtojhl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxrwbyjs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rhnvxtwf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3sxbqopha.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atdlboqo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sznoihbw.html


<!-- 参考信息 -->