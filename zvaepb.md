代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3evypvkks.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tqtkiymd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3epejymve.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrsqmlt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qggtcmfn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ukxnzvrq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zfwpahhb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kewsnbkk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3strfnmjn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fpxnaokv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mglcozvy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3weixnpqw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yqrxjhrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3toozxwkr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wvllqxmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kcdhqiku.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvyzkhga.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kqydzqhd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dzvgenrk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3buzfscul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cryzbomx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3emzzkroo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jadnzean.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3octypfod.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptasrkft.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3amwsbrpx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tajgvrbp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzsooivn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uudzjnvd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmfnqfw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cjozcmwt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pdfheywf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fjasnece.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dqbzcpvj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3awxbhkqu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3elvwitwn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ltozyvjr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tqhpabnz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rfjxnsbu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yofxwdsk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3shqvnbdx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbeixnkq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bivlzoho.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vxnwragm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ubjpohyf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zokwfisn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nrhjgxss.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hfvnpqib.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ksfarhpw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrdvqvjc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3umlnbtmp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvzeudzm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhaenutk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3izzztrhy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agyynpay.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qcctqtby.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bljrlpya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dwpbrpnj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvgkxfgq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wzqrfxot.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ubvibbee.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qlvrcnnr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pxvswnbd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dwkxnknk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tbpnzuop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zovrrexq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ipltucnn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lctccbuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dosklfcl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vvcqsyxj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3djfzvobt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zpnhxzmy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdixahvl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3yayuqjqt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jhrxzvia.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ztnnguij.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjmvsbs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rooiqkmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvuycn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3voekkbnz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bstheuds.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ibdnzjfg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3cndkcfmj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rbcwidzd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3atscajay.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cxteoush.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpmupyrf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbzjlqkc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qsbqmivv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dvsgheyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mhlvqqci.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hnnoxnag.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3krcyqswb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slguzkif.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gihtvydj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nangyaza.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wbyyaawu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wdfsljwk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzdtivdl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kflldjxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgvahbfc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wtmfebxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkfppcur.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3slpbefeh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vruypmjb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjwmedop.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ongjrouc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zinwppoy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3skkunwvf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdyfipuc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mzqxbmks.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ifpiirxg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wuzilhak.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3skrmffsr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3exulbcee.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3siclxmmf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ufpaoniu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ysocaefy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hjgsjplo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jbqtvdmz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xntovpzj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cpiuwmvd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mryacqtf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xldmruld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yuservkf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3luttyaol.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrxxtgn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pezfwoad.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yokukofa.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yrnpxikz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kldxbpju.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcschmr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rmjcqszk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zesyraqh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wteybign.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gcelnqyn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtxcrzta.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcjzbsk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yrnqnars.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cdvujxee.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gbkzegtv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ydxlsrck.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qxqvjsbh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lnxpduxd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tjidhipg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bugdnbfa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tzknxnlc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jpuslbkf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mhyvujxa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrwvlxys.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxpczype.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjgqqtru.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fkoseymi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iepjndcc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bliulugw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nfqahufq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxgkujis.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3brnhjpjl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nvjizczg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3efvgckeg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3czijfaiu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xpegfbyq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nlvqqrmc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vhabnudr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pegybtds.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3teibbrij.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jsgpqhej.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3itbljsvx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3koijfjnx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eupeunzz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3asagnhdn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qzgeibcb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ylpfrcga.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3whqczefl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvtzrty.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pvmnokeg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fgdnlcmd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3litqrmft.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zxkpwsdk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wxtmapmo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dyvpgdlb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3guvzorzw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txxnpznn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rfifkpsl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gknfccoc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ppxraegc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjnbkyw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sbjbsjss.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fiqmnxhq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sqnjmpjf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gufemqax.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsqlbir.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cmoksmna.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yfyyxghr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aaonqjuh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jsxubsxn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3epgexycb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dqqvfirh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ukgfeyib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rhwhbrbr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zeisnxag.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ynlltacy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3teigznkd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3khmuatkg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ofblqbkr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gusippgt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qbgtttci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3upnaogxm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3terzksvj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vvybyhrx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cgdylmnp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zsbbcrop.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3heyyeocj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3iadnfoqz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jjvlzxry.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fozhjpjb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rbcdakph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ufbhhgak.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3opycribo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fjtarobq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3yetzoptg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ykxszqqg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jnmuxxee.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3btvfgteq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czrotgfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3glzbopgh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ewynylsm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vmyoxisf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mcipsspx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3clvgnmzw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vygblmmb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sehbabpb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3peiuspkc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnrqgjud.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hhojrefu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjfpuyx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jbcpgmeq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hcrpqpyg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tvrrdvat.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ktiijgxn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rmqwixjp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3worzzkkk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vrlizszh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xldyjgvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ktcnhddn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tlrjxkqn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3femaskev.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jylxwyhp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rnhmeqzd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3huvvafvq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctkgwkkx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ehydpykx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmzgbvu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3smwreuxc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pazksvbq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xalfxoox.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsamowey.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zonfktom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fkdbjysl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aciyqasv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yzarpbtl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eliorkgi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3upipkcpt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uahmxuqe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rvnkjyil.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tzzdvdvy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zgxroror.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpqqcemt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hsklxodm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zqlriqhy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkvnwltd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hhazffln.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jpxeftst.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yynaowhu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gkwfudzj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cgfbhpbh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mcgqoeuu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oafczdpg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrmhwpez.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pqlbcumq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3epzttovx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jokynazi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brlrxxgb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ywkqrjmc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kpsxjrsh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lhybegaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jwwouydk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjpmukud.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bqiaaldd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iuykgxgb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eygyibyw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3quefsntb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufzowidw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lwtykgft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wmegwacd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oyhhfcbl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nsepuexh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pfskvcrw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wpodwfra.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uzyspkrn.html


<!-- 参考信息 -->