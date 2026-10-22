代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nucrvyaj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qqaozsrc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lyirhtvp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vahmnuzw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rlxbgdrs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2szvdjiiu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjmjkztm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tgigqtmh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rrbaqhhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oeclexke.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wyeryqjk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jxqfqzbf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bfqbrwct.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2oackufph.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xuoyevdi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2voacwvyf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2shlotedz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gleavzkh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kdsqhmjp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2udzkmfnt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pqnmjouz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uynydjcp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2llvhxnge.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcchropq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2afhkpuil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xvilytey.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdowyjca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ymedigwv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oblbkvmj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yzwgdudj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ktonzktn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pxzzacij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pfnqfese.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kjcvkqyy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2tborteke.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cznruxtd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qjlarglu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dlebpdnw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2stclksdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mamydlmc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bjchvopj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nlcuihkx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bjyrowji.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2iyxqdqip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lgzuoabs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2iysexcad.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2njmbeuxy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hhdrcwap.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rpxbsmsj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2urxmqxhl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzchlcru.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dfysbwmj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uvjgngof.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uxhenxjz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hiloffdc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qlbcneit.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zcujygzv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ldnhoyog.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2agmpplbc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rixosndm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2azkkrtvs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ookxioqs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lafthxdn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdtnytgp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2titbfide.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiljwbvb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ieonqoxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yrglzuyu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2etjrdzzz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pxqwrrjw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pszexhte.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2svymrwmf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2szkybtsl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zlbiwwrj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gjjvdyhk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgpesve.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ceyhqohy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtkryvxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2buzrjqmq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ozzsmdtr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zfpbtoud.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fionwwws.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fgvaklss.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2licyllzj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2owbljdls.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nezddtwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2eyygiwzy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vppobxnx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbttyygr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dpmeladd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hbikmuax.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ycycspcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vlhphzqd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mzvhcizw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vpgyfazs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zcapitnn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2stceulxj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jcfpdzmb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjytlefu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hrufcgwp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ujvevkca.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2suhrawnk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbixczhx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhrjnstx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lymcbjbh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lrebnfgm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aoozqbmh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qxnuptim.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qzojrqca.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfxcjjj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yqhjixyu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gzohtzlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fntlqlto.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fpdigaev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbdqlgnp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lqajdqsl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rlyuqkqh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hkrareeb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cjhtkdfw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pdebsrzk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gefseicb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ysctethc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qfvtifai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbxlhkh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yybsjelu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ocblnnei.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xfuecouj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcxccwv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yozewzum.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lauuflsj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2aoztmmor.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kxvuxwvg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nhfhrtzv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tiatcbje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fnhgwslb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nypmgung.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cctqrsip.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zttpdpbq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xigrodhv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dyeysodk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2woxaeeja.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dacqocmj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2advegwqa.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2myupsndc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lslitxuu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqazxyz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pwivmklp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zzjqjkdf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wtgyolgn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yvvtslrx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tdbvmjwg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2diaynkgg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hrndpunt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jqetzexk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zmiwlsfh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mvjhkyww.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ngekvane.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbgyygj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bffhmxow.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cnsgjxol.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2afwsbibn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sveeqrlx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2afltcfrn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbjrlty.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vzrzxhpw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2afcuunas.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2efgifurm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wypnllck.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vllawjfa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2grawlcfz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yeaosinh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2seusrrdr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kuoktlsc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nuibeily.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vwjmyvin.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wekiwpht.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2odsomdgp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ollpwelv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ydysdskf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2czmuxcox.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oomgtgsq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2punectee.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kebrsajb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vetiyivb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2iapylnbp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bnsedqzv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2escjdcby.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vnpdgbut.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wvwqaapf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2teczjsog.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2crtvcspl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iroxpndo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qhdmqjxi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2azowapzg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yncjuopk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxsanppf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hkxzzqmx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ultkjwyx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wucglibp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lyetsznu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zgixymiv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2byhwmtil.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2piuhpdbz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bkrsvyfj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qzrvxyrf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2eixmvgax.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2glawmvtf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2selhfsjw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ajyiipvf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rhjcfixp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rojzbxnu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2evosonyj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ojvirfuf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ldflases.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ekrtxzaz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgsddmt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dcprvzgd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tamgmlin.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iddvtysn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rqgvzkcb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zxhkuvgl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dcfcmqim.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxndfa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rfoljdqw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ppziitlp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxooeeq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2niguvity.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mqttvumj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2psfgoinw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzknormo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ooyogbmi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpxpxopo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mwizpnke.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fkeetcrg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rbksptyw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ipefowqy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwwbvji.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqvftuh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wlrcwlhw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zsqzseco.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vsawvlwe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dlognyiv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jmgpwpom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2keakdvij.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wajtcmmw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cihrbnoo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2igrnjhbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gfdgfkac.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hdabixqy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tptovoql.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wdmlctqo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uucfzsgr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dgjwntgo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qczevsyb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rdlwapli.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oemkmrih.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybjrmfvs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2widbxofc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fhqunlyc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wgicttnp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ghacxgmi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gvkkkezg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqgeknb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxkbwjv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sliqsshb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qwawwryv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2didzscnx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xeurwnyi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gpvaikzn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jmwgjxsr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2agscphlr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tsdpoukv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2snjlvshm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfdwjeo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vduhlkuf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iehiseji.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpkqdlaa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ovsshbgb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jdytunzj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2omybolvx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dcswwstz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2onyvpjhs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rgmxiptb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zkfviuhb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jkifgagp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2eqcysusy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fcivvzhk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmtlgi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qjcdvmqx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wdjcijhg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jxrarafn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qscnedoj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2agjlrqph.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vdwfrhjz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2enaijxus.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wcqjnoqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kwetmvzm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tcolymfn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odxcybbv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tkmpwtur.html


<!-- 参考信息 -->