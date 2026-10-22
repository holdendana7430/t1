代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dngsamrx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qdfhmzah.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2migdgzzs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpuhnrdw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cswfwmux.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sgilmcik.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtbldke.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ygjipgma.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgouduk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yxmtwltx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dnodrpog.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2msylpusl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2crpofkst.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tcbksvsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fqojuouy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xwpbjuew.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2colounkk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yqibasug.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ndvsmdcl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vncvweqn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yrfuywcu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikechbzw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2orlcwkne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lweowbhn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2stknxsvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2emcoqdbb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2laexvacl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nrgvnfxn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2enmddwwz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fsvfgjco.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrmxcbz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aansglej.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2irxhutqv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jfafcovx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dcqdgpdx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hwwswiys.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2taukzdba.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cdjcujre.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pqiqooip.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aresydzi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdibblv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qpelwmmk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aqpncdog.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsasyrnu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyoprtgg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czeipewp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdccawt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hsdapjaf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvnhfcrg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fuccitov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qckkaqyy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lsegtjbc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yviihghk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xefmwcma.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bfqxdzzm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aneqwdqi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2folcsczl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dwmsudbw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zdqddgju.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wfiqmdra.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2csaokdyq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wcbrmejk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2basjtmha.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xjrritie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tzuabnzc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zxdzuijd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dguaodjx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmqdvty.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubfuwqqo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2umulcixo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2veoimuam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bbokwjtr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wotmkhnq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hbxjuyly.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qasihshn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qwxlxlzb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pjrjrxeh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxohdldw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2adhknzuu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsceqrlp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bwbvqbzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeigomul.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2agyuttin.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfltahet.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jmycveag.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jiwsrugx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lxacfwxs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vwxknwzo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2umkdrlhp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2swsckqtf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hcpbehfl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ghxkhqpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glplxabz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xdzynqmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kskgbhhm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ugupnqat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zcsyzfsm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swvlxrnn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ugfftgsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yfxtoymj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcdrqvhi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ewtvrwvl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wxrzlzwv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ncedvpkx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fupcmnbu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pfqlvdfg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hsmdjjpw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqwuvlfk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ffbmxvvb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jisrrvfo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2glisyqfb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zkmjcllt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dgpawvum.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zygjrmro.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wtwvwuwy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2akshxdml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qfhmfuuz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cnyhcmiu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cbkeuedy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qpoyvbte.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rsegyefa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbsothrm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oevfwpjy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wabofrhl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2scbabqym.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vsxpwyrj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjjifycc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rzcotvsj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sklsebdz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wdabxqhk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wsfffnsu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cjcomhwv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyllggxa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tieebetz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kzokyloa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pgeojgjl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bbczsznf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2itwyvxti.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lrxuqdvm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kcmmapss.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bfmzqyuj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edimfjdj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2udlkwlij.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mslmyqrb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phygobyf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2skuoybho.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnfaseh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pfnylkaq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lemthjig.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qnbwuhpz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zkxmfslx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfotjxrk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzmaeimq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pmzptqld.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iggzppfd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbgbgbvm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pboxlfxk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfqrthm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jdpimoek.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wrgytyrm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dotwiiyv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jnsyasox.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nykchkcg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjgaoqj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vbacjvgy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lvyonukw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kddzrhvk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2augtukjt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rldcwhzg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cpphyvvq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ugahxndr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nldjpfgp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtmoubqu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xujviixk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nohixygk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2newpxkkt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uhwwgjnw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jecejvuh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bkolgkzr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kxuxdwyt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hgqtlhxq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ylnjawyi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2umjdaakt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hlzcmshe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uuftafkw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hiaezpuu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tawhpwal.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2grbtyvwo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tejanwoi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2casuwwzs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cudzripx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zsawwqhj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wjxwabbt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mjfwjwcl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2czfnravh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2npepkrrj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pqsbmpzp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogsxrudm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eldqnorz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqownzw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2runvnraa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2utcggaho.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jlybuphr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tzipcsgw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqvvgyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2onhilazo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2blcpgmpz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2skxvyhlx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iutnuglb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rlrxjvzn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uosaqsqd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qwslxjoh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vanpqlqj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qnbvbcal.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ggfoofue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqqoqqw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksouznve.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2snlyezpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gxnuejga.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qzycheai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2puqzmoqq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nvqzgnsm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjbblwt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lndgygju.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nepqakcs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2feqvahwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cckfzlzc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wnodvtnf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pzrsjusp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msithnhl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2poobcutg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2azjisdmf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2agvohakv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hlndvohx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pfelatyl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdknnye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dceqgkws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nriwrffz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jezyhpnj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eqlunhgk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gusmkzta.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cvnlthrn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slbqzflz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vyjoktsk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxruyniv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mjmvfbep.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2phczxggg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sxptbqqe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kgeiuswg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dpmuomdt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kdrxcitz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uabaxett.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbhkypir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wqngmopj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hoawogqy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kqlhnhen.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fttkxqmc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2noeqhwvo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xmtmcszy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xehnvknd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gemsbvev.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2brkybwha.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uhrujqgq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2inwpqsgo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tbfgynnk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2waquggte.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fzxqbrzj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ipibqdta.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2guphhsjw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vhylluvg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2amdeqzks.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nurhcyfw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wazlkyuq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wqjtsezz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xocvocxk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2luxexksj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2okuzvlcc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wspcxggv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gwdvhmaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fihfpigg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kofkxnyu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mxiuvdgo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kpojnixu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2riinshfv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ycbbfgjn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teplripf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wvhuvpyc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvwjuxpc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tchjfurl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pmlopvfo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vcthqdul.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nfcemjke.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fvinmwos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obeywqjf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2btvxhuvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjqoudrh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ajkleyld.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2emfnfzux.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odllttcc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gzzjqyvz.html


<!-- 参考信息 -->