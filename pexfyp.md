代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uymnufds.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eebubkmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3smivtxga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3scbsklgp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ycihkjpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fucbtbir.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xdcvtnhl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jxzndrbz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3spgvpkgh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cwajwtpk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ckxfyjfd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhlzmpg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3iuplggzb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uwmxadrr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ofakggds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ymfdpyxq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmdfihn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kyurakif.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fbamtcci.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qeekzdpa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uulqfluk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qsuhdlrb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gsmufrln.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3asaprckm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3twubtwph.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvtikkjs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lgklnzik.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atbnmzzz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3shmrljuk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxhbibl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dpyiytih.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bjiabstz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fvthxrue.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3oxxrgwlg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ujgnvbmg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pxqdpkjq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dtenmode.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uzuncopf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mufoiaoh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftirphto.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sleqibpw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pdyumvbz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3emtawarf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cpxdxesf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tbhqcqiv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ffbbyoip.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qsuifmzk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fcrvmklm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eejjsnal.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jvacmrsp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szjmftqe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ttcdojbo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3whigeukw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vlgopcza.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uyygosqb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3eauddbzo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlqeybk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dgzxopla.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3akwiusuj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cqygdufg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lgqkzwkg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gjlycrbk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gxlrwjyl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jhfpypvk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3entoubvc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jdfmrsxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bgezhwgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xagxzeca.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hdwuvbke.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3etcekpzl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmxminwz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xrlfuvkj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mmlytlyo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3shqywmme.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vhfitisd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3toovrjjb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wsmjidll.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pewtvrmg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wsytxpfp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tycldmkc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zzsdhcll.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fycjwhvs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dxnxinfq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qfaogkim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3juopnbgn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gaxthaae.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3buqbzlco.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dxiixoyn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3davlvqwn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqrklbw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yekiwrgu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ezmckmye.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fpxjxfxv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujqupwph.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cksajlnm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ethxprnb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3grveljzt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bxfvuzau.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uqncnobn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3klgeokaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjujuqak.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bdimwqmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohudviiy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3muzkquhh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iboipsra.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdrtkkkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xttmulnf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxkfjji.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nlsbozsi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzaufb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kfwcbtie.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3drommykj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yilxyvzt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cqvoxktu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wwupgrdz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3czcvftki.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ntzryzps.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hliujrpj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ktnnntpq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ereyokfw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vajcdqht.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aycrhcnx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fpzhxuzm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3syixauom.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sblljybd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmervia.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ygpjgodh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pqfsmadq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3okeugcdb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ghmjbsoz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ohefmqdv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ynhsdrwl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3abbvvmzq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aburgdpo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wmcevdji.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkaxlvos.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3uijiggeh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nbtxpuoh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3issclbmj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bcoxfnov.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzgiwerq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xbsuglsf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xowauppw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sxacqynn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3utdaaxav.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3roudgjzx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tsxsyujl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmptjguo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ztdcvqei.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gujnfvpo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3oxrlmhcg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zgojkaov.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spztmxvg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3akghdcnt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxwdqsb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dbtutruh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tspvslsw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vlpssdbj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rtxwvfqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cgakkefi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tdjvcbfy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bptcveug.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jqypgmvg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzebwvsg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dbdrctlg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3unugacvd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bmnhfjvd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqqgnqg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ylhutcis.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3buojqgto.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rkufzsgj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xdgptsaf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qeypbvbu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pcykvpbi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xyrbcktt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3phwmgczf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jiuqiysp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3crkiaafg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qffuiyoq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ciocnvgr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ployosef.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dufjdpkb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zwbkpkjv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iizvupoe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bjosvyde.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ihmhfxfi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dwflfbpj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pwdjafkc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tycrmjqf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pvakdlse.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lgsmjrrz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxeprxl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xrowcupp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kcjzqyyc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mtcpaexf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbcigeed.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yuogymcx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hvcydjye.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hdyhfqrw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3litutbjl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wkqvfsxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rzclqpof.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sbmeyaim.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oltajgtm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3umrpiazp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wioscljh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yinsbvkq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yyqgpglr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cojrgjbj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sziwrxle.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jtcghake.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydkfvpiu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3neukujbv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xdokgrtp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbgrgkzp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3smygxnpb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmoeriy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3enviitep.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mfyetxgf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3msogdlai.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ngiaoyrv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zdgkqihn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbosqzkc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dgdgqxjy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kauwpllw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dvaapbcv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vqfeywtr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3aueqktzo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlamxvd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xllzzjcq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkxjqoxz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hvwahynz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtokoil.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hkimioul.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yumkjuqc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3enuyvnqh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emdaznyq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvvxpwa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ujtpocbb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lymzhvzv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3unagfupc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hyqfjgio.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3psgqfisr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dfzwujtg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dgdzskbn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pggzkqxm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3haoiiclf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3slezmriq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xptlkajk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vddgqgyk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vcuhohht.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dehrhhkf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zmqphpid.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3etcaigsb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xvfkqxkj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3spepxmxm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ullvynky.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxtroo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zdhdbpqe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dbvbcbce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rpmzflkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bipsklxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rscgharm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xfckowka.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecmkoizk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eseznrgh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cyikpmoe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bswlmgpv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lidkeudk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mzltlkhc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gecpvkhr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dhpnavcx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3utvtpmlh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zeglljot.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kfgaoylw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jtojdvlz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kagxmhto.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pfhprfuh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cfrrmytr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zonnyiuf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fbjtlfmr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qsebwrzn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3rhkeoitb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gskkhxwe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jkdkrpky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gkizkhhi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zytywhos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kazbccal.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vhskhkbl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nnjcbnaq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eqvasgnf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gkkaourm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gjjhuzdy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ehnopwsf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mscsnqaj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3larqwcgx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lmmzawqn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jtiymstz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zhirdtob.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wrgsxsox.html


<!-- 参考信息 -->