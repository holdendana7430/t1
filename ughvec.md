代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ckrtqcpz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tzairljd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjhjagc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyjbxfob.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhvsyak.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2epizohlj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2usvqjmxd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wxbuarnv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kawjtmtg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cuitceld.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fdqypsnn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2orgfempz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ymkgnlfs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fomwplea.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hvwhcesn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sdkmubey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xugiuynw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jnxvfawx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dnnmzaoh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kfvjbmff.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cfmoubuy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kzqlaxay.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmphmbe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rmmdkbsk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfbgbok.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fphngazx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qlpccygb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbmbuexc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hqyunmcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hpzfnpjh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2medbuyxp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qrouwajl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tpxwkuhm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bkeuwend.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mzsorcuq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yqwgdxmm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yvthhmao.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xzzraged.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwgukbzx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxxmeuh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2abxguhyq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2njiswjyn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hnqfberf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zvarsjvj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tlspwvrq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cfzbanhr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sihaykot.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bvkftpvb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2unftankx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2keaygsci.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkeaqvsm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbtkdfz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nfpbxtor.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2deesfgfv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vaouoayd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qbvukmgm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yietlcpj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2rwmqunqx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tupgikwf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2esmldwwq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2weexbuyg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2malacpcw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2djumvqjq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mvrvbgwn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lmzmsmpk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qomminiu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nznlqdsw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2osdakyfs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qvmdmtgf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oslzppvk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2phsbsopo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tqmoblvm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ziizzyuz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zqcmlbrs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pdpewfzk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ocfzjsgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hhjqextp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kzdncomk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lolbpwut.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2susnzrnk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vajyjjbz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tqmonvgj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dthcawkf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qzvrkkvu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2blrnmoaq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbktsmm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zefahgyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uljddhif.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ltxexubr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bjvcidex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vpfxyoav.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yoduecsj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mszrwubb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hxrbtkam.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcdlxc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mikupdjf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nplfyogt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgidvc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2spnmfyob.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qqiypive.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjfhugqj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mdufvtis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnudcohu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zoxopvqy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xpcsmwoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vvvrcgnj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mcjyoisa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2umsfvjbb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ntaqpyjl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2llslfhqg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2deelzvdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgxuemhv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hskgsjof.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dvjlyrre.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwanti.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dyygzeer.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpqhbgl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dumldabf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hbymzvwz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ekulajfk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2blovpono.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hnhrvmzv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2phtjlaja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ogdzlehl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgdzjvst.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sucxzmyp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yriumveo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jmbbafwa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jnmybtgq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgfxvx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dgjvapop.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vogmzaxq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ktsjpwlv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ypprocpn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qvkrvejp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aenwjvcf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdwxqjsi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gshyoxib.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2npjsmzkv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hkzzdqpo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wisoiatm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2egepxqhz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bagvnwjv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jckzecjz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dnddrrrx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qwnibjda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ybncezpy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pqldrxqh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jpktegfj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjiomrmf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wnoarhyz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqonumqp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kvnyqgug.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2efhyekrk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nonilmab.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lpqdsuud.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2psanufhe.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cidesuhg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tkkzkxsr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rnausxgh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aecbzqnc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2shvvmowf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tvmppmjq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oogsczmq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hfnptroh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lkwqwfwt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2spkaarus.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2scavaeuq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2swjmkctg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wqpclumo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mhsqfyse.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ylmzysgw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xczpjyfk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ofckxlco.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pyzaftmj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2unzkzxsr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2baghtune.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdazhkck.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2htmjteex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbiejule.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lculcvbk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vzdlfvlw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zdljryoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2svwyxdrq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vpsxfwpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2inylwsan.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2llxvmmsd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdorfur.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bekzwsyw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdltqde.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wygzhmpy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oagtvcar.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ddeicfse.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tatqjhea.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jnumwrtp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddbxnnhg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uybbxbqc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wymofsqr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzeesegn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2loccymhl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpgiadyv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2udkbdcho.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2icqgbrvj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2osqphart.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zencapmw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2meqdvyvm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzvijslm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2udbrgijh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jxelirgx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2axmxaavy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dzmmajsq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rwaewkue.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yidocncy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mtpgweva.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsajkrug.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2benbymgg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ewhoygpe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eebrnexc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yegwszok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkvuvlma.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ykcwyznj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yzqqlgep.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tlpxzuwx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2etfktkwb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojcekrua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kavuusxj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2prghurnn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nwbyaovy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrezbqr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pwhfzgvp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nkkaydrp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tmfjqvtt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtkmyhj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ermzlhsx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wcecsuoz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ejxviqay.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fklalvlf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tahzttsl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kwcwcwqa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sidauudt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2szyzbsbp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wsaeenoq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qkdzrzpj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2maunftke.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hlgwrobk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xcawqlsa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pkjqpkpe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bnvzhmgc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hyrunrfa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cbzpmpiu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufslieqd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2deyyvcdh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmjzkht.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lljazmtb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pmqcrjtg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cgodeznv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xbuwiyhf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eqfgjoeq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ashofpnc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ijwtisnk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mjnobjzs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hkkkvclf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kjnyfbyb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qaqrkzew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wyyhbwhc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qigecuqt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lbhohapt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqgmfnta.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2seqotxqy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtyirbd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vjpaagmd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qrrcghiq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ejannzgs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kvnpjwzt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2efkyaijw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uqfejfmu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ycbnbarn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rfivjsxn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2seosgzbb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bamdrugr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsqkvhph.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2llierzwi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpiggojo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lwbdbfyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cejcwono.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2szxlkaez.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hvkuldys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rcmzfhio.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rcmbdsoy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ppzypagm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ivgizqox.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jvcdpisd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xooqwhiu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kswcakqi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vmjdvzru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hiilxdof.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qudwvcjd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aznuakot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sqmuaade.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2drukvskh.html


<!-- 参考信息 -->