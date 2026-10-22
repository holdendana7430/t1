代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rfggknuz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmqyeoqf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2haxxpznm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vbuwpeew.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xrccbdmw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2huicogqj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dfxjhzix.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hnudrffb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kzxlkvka.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zgqvjrrd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qefgzvya.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmhgdvpr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nfkzsxar.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jhsrpmeb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kpjbmveh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2frooyhvw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tklgzntc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pguxyoyt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zwhjjwnu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wcvzvdbu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cfjngtzh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fopzqbfy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ofgpzfhc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqtfwtbj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjuqvisf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2duaglzek.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jeproyaz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hojjttzy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yncadikn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kmojgqaz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2agcncoko.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dqbbnrrn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lslsgplk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iwdvqxpq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2znxsnich.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eprrcyoa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bfkirrlh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vkpzepda.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2eqxptirg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tejgdlae.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uhviosbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2azpcpwew.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2trqedktu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2joqwkbop.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ebplsggi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tpifjqny.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ayyxkuru.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jnmavbmy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuubjkyt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vxjoptgw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lnfwciuf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nxvtrnkv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zdrondhj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ovgskgsa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xzepxbny.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2sfpcedyc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kwctvfkr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjiwltd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2myzxuzby.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qvpitetz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2udqqlhlr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mecspdtf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvxbwzz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfwvhpsn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2stqcrivj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vuermkrd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rijycxdk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nwkiyuqz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhdecsl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wunobdzr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tmjbdush.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vocmihzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwbkcqqb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xozxzepb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxfdkyty.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eugtjofq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rioqmyvp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bsopqyrt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nfwopamq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ecaaqlht.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yeggcfen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pyeounqv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tskwajox.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rljhjuhw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2easqdiuw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bfpgsrnf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ximnepmv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2skhyyqur.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bmqrtapy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ioypgwxu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2elfvflpz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hkapcuzz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kodisude.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kavshhja.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yuokrfgo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mhrcvevn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tovpsfao.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xxuxstgd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dvjgomak.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2utbuiwrj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lvylqfgt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjuyrygv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fgkwzrho.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eacoflbp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qxgqpkve.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bqpfsvsm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vkxllkgj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wplwrlvk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2krxqgbbe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2phndwpwy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qeqbupzc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2lhsfebiq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qnnqqrbt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2entdtqfv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqcnetkn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2psamvsfq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zhgpjujj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2iguulaan.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iexbqbbd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhyreug.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gfdavnop.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lycdmfoy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpctltqz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2neizvqnk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nknmvsui.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwydnnp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjictws.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2leozefvq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wyiyuptl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hkjlrsbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fohoexbj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oyixziba.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2buajkxio.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gndnacyx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kwuadjhq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtcpuypq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iwwlaigt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bumtwllf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ebhftvpz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2spgufqdz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2abldbnkl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rplnvyks.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dnuxeysz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjzrbbb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2urgpxzgm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxepsko.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2brymkapd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cpgrmcyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzsolbvq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tpqsaxev.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmtoaju.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mwiuzdiq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2btkynwzb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2akckhgyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2seksaifc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qcyogwsd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fufiogbi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2weeqdazs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wpoouuxv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2anifwxyt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kofjojgf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kbonnajf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zwchvnei.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kbzcivqx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rhasiuss.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ykgdwdkc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nusnakvn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2maagnsig.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bfjrzgrr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mcjyoejc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jrwdksdu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xvvwsmjq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mizhxndm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mliktltn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xbpkqtju.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2thrdyjcv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2utqmsktx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lwtrovfu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zvcywrkc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kirbtxkn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgyelhue.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ifahhuxs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2sjtkrglb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qzefreum.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kxoaowgf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wpwecodw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbeprekg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kemtwqzk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zxqtmgio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2etisotyn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iboymzsx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fckzffei.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zwzsgkgu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kzvossze.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxdyuy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sfyhzzcq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfuqmmok.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cwobmkhw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nukiwetd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rihynuab.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mymcjpcr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2twkjhwdp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tzeklacq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vrmlycde.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzngxsm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydtmywnn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2orfestbz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vzkjtoos.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zufnihlv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2npbfrlst.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghhljyrs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nvbgexny.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pxqlfjlc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uqpqzlfx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tmouudjp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vjajzvhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tuhwgxqb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cyuqserr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ptovxbxs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ztqrwojs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bghdrynf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2joutmbdx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldfvrsci.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mqdwfnbn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uoixzwmz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hyzavwrx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pkxujpqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jrpygbki.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sysdkxpe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uxsrloid.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mahflina.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2svnmwgdg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2djkbdtmc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nbasopcq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aasddfni.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrpvwziq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jtmroyuv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2grhgixpv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wsosfebp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zmzlnvpe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ctsifxbp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sbywkeac.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kfznyvap.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sfhyjimb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gydhvjvv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vlnklose.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2axtltzyv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2afremcfg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yavkwcnj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2eakkdjle.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcveaaom.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zvqfhwvl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wfveqgyi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ztravtvr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qobeznrz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2prukinaf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2duvgrhhb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eickninb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jvgawcfv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hlpcxxmq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gmuxcqik.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mtnkzkkg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2czdvhbag.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uakgefdg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hqsodcpp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2iiffphsl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2onqtsgnj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2niylwnmj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2agjiywbt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xwbujscw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ndoxyudd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mulajgze.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wagaefic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2towxnmre.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2voiftdbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smfiintb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcaqbkku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ltuibskp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evrxeppg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ybkerhrt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2whgjwcrk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qypcnreq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nkczgmtg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ioyyuyam.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmgbawhz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijbnllrz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jiltrbzb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvthkqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egbakgiv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxpuvqnu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cpdqqtdt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2onnldomi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zutzwyft.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mjsrbuyd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ahzqmemo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jkukmyto.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sxcfyzsu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gsllzuxu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqicqqtx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vjmawyxq.html


<!-- 参考信息 -->