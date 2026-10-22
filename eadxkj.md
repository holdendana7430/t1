代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcdnusrg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvttduxd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zfihtdfy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2zugnegon.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2feezrtbk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2knnkmslc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ltbggwen.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hgtkhzys.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dskzdgen.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2clxwyuxk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2awnbxcne.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2voxpdweb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gbdnniyz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ucikdkia.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iajxsojz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixffgqrc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gdkwdtbr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mukoxtnu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2exfmcflg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nkmqbltc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2huooitid.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pwadesii.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nlhzuary.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vmlsvguc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uwqiykcb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mqgckyre.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tcnqiygr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxgitryy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2togqpfdq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pswcqfyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cfsmdyer.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qiioqrqb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2egipcbnk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tjtbinow.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qdrkzgxa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jzialagh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zenpqwmj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wutgoodr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2meinxyjf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2exzkiwns.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgsnise.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djmyudsv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erwkvgez.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2blkgdjkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxtoqexz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vcpzmkms.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abhzftrw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zokiwkgp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kwbbjvbl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2frmaqlfc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2axwbcgmf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hajknxqr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2gyfvhzql.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gbzszqdk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adcgkvtd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cikradrc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpudqxdq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jqovhvfo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fatbpvfe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ubprfdcl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jbspfshi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2kdpkqzqm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2itdmksux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmpbadco.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cedpedae.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jcrklcpm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nebbrvjo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hndlgnex.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2syapqgnb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xwovqvdg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gqtyyaad.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jsbojjby.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cwgquqts.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drdrzzju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ntnuqmag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zuozoomr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tjvshlcy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2snuccfio.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xqcntasp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vvljlqer.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pepkypvb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jucedtht.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bgiwhzbq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ymwggcdj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ihpswwty.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2btngsdqv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ronsojaf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xmfvmhvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueklcpzw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tgxttkcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzdcfwzc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbirdzxf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kpyzrgml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2emiyxnvc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqcbmxwl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zwibamyw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ojhainxi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qgoevqis.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2isqptzxk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssooycml.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqvuiizk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jwjuiviz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pmqmbpqz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2borjwcca.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsvybts.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2myourftk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijedftjh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qlirnlaa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nclcbrws.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tpjvvset.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pjnmfdsp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2doquldlk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmggwox.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hezfndlk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdqhhbk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gxrdgxxv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kqrxcctj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dkwovboi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kwfznsor.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nabkgtfu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pvokzrsk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2csohvimq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jymhmaoz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zyacjlqq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gqwiytej.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kqrjzhzc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdzsjcvd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fukbfhfv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozrxnzrh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sdtsofuy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jwqyumqx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bymexniu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkzynph.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsxivsng.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dzajdoft.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ztpuviak.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qfbhhomi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mougoxki.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rpvysjtg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yqvjqkyr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vdytmjxj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cylddadl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzywkzj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fkeijgqr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kyoytqrx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zfdtxcmt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cutttqal.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pyosyrwq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mrcwpxvo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rmczwqyq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ifqbkrcg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nqrfqwez.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2viohjcst.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmwfglb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kcwylmpj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2srmaxyfx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pfopjuep.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pamsdtss.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylfdotww.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2daudxzbl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2awthvcmv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqilagyh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hbfhfdwd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gouvnquv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yrkoyxrx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbltaee.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2illqijvn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cogoondn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jswqvikm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2izytzeyk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2djgdpsir.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zmdbfqgn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hqotexlu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xpjfrapo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qonmgmfu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nukvxnpq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cbybexpa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbeyetb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hjhzdcxh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jbacarra.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2trtxgrsx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qkujanmr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mrdljcow.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fukembew.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfxnbfy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ungddbnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vdeqqart.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xgavkekr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rnavrlwt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qientdxf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hbvkzvnh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2souowpqa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2niublrlj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dacvirpm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2srcewkvf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bezaqgdp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2koigqtqe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uamktidk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gqnqnyqb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iujrfqwe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qcdkxbzc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmvzzul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vumdnqoj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlwonyr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2czfnmwyf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqixkfnt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2azgcqnxa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tpvhmtxp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2brwqcsuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2egvbjpwr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwslyhvr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bbmoipgd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okdfqrne.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iyyqpgtm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gczehfyz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2eeprmkxz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pkyyiqbf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sehikdfb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hccrqueh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqrtvjve.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rdakqwlq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2totytsrx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2szfztwhq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wwfwdgmt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvvisfj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ujpdmvcy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lssjhxtb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yotvtajb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mysskblj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rshlqhzx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zfkdnyvd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ztggquvf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aoassncb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2atsrvitc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zragqvmx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zakqjspl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ytrebstn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2npxiuiee.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tdeemhjg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qjiwpvto.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eazxwauk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kcsmrjzv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2solziepx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dpnbaido.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lyfyixdr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nowmmzjh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tktooexf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2snmlkdch.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxmffkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fpwdslyz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtjkxvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mrcfeenp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdhvsvjr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aozzylod.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xoewyhvk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xpanseen.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bdunbfsv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qjtyuupm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znsshivr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvpjvh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2swpcnhun.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dikxkppn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sqsfydju.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bbfdripm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uaycsheg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jsmapgic.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmmuntwn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdrgejeu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mldtejxz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qtugdwdy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgkbnuzc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xwrlcegz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bcqilekz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cqgqlnak.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhivjc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmmjsjjm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zlgwgzzs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yifrszpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jwufrfqs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cxpehjbq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fhsrloib.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kehpmjgo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2szqbldtm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2youijszf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qdempjuu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tgxwjyqx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2frkcizxm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hkmruufq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vhbqjzqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daxfmtoo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ubyymcms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgsxzdld.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ceilcwgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qhfhfupb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2byczlvmn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dtlvjbyz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2waamiroq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivskfcvw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jfdtxvdj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyreqdhh.html


<!-- 参考信息 -->