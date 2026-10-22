代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2twsrixxj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtynhqnz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkgojnqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iodcytpp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2atdskhev.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzllvmwi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evajdsgq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hljucdpf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2veutepik.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hioiblva.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogjrhdnh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ithrdjwk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2btarptej.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gqozzfyk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbbyyou.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2njftltsz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fkzpppuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qtsafryd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zwtyubew.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dvqunpcz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xjocqlww.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qjnrwzin.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfgdixop.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzbuoawq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfmkwgfv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2beoydgfk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wbtbggmo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kdujtwoi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xuipiwez.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lzgnivuf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2trvrlbuv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgjxiha.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isofvhwt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vrwmlafy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xkhvqpyj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2omuqidgn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrpozzkj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2affdbqpf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmvwysi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qglvnzjz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xlcuozsd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vkipsjty.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zjcxxcfv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kdlqmowy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2trbyndkb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrbjtdim.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2slhphies.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yitdakkn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xuywfrff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxprsbl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jektetdc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ivqhcsde.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2abvgejpy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tcxkjuov.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zqplwhoq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ojerusui.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vudvdsug.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uncxtqmn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmkttpkx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhlqinxt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2reztqhqw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dryikohk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vnrsrter.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wezxzohq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tvisjxyd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cpdthter.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ehhyirqa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qzgzrllq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vsswftlm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2udfsmuql.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xtzfwxdk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2usxauaqi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hikqrprq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2apglantf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olngblck.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wrmoqzey.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dickwegw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ztamvlpp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2btoxjezo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ahitubrm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2utxalggq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2leywixgk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zrhpeuve.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nkbjtvla.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iwmjtaqz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2taqawkcf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mhkclisr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pftknvsv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uqesuvmj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aasflguz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqbwlkiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kezsjmmu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mwxfewre.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zetehnoe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhhbgqnd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2onvryaht.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehiqszkn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hnvzbulw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2riycganh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oavrocme.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mkpzsjpx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cdvrosbn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kfgeffci.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wolykjnw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cyyltlex.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2cokeyvjo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2etfhcibx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sxahgfxs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cykityxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cizoibjj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2boofsgjw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbwtrxus.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xfouhxgw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdjcqqbp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vbamweys.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pgwaybhk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ctjywzzd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2getxaukd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2anhcvcsz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvxwxiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxlwmokh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jsvmxzwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovtumbho.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xrqboddd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ycekoyzl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2idihjfcs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xlluzdcg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2znxvbgyi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eezdlodz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cswudsir.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ygvlozjq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gckykthv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tzpfrpqx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2shutjewb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zdrxnnaw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnoiain.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tfsfruhn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2whoyivkh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cuagtils.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tsoimdhk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aueqzocs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dlikjctt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tdmviytf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2trwshfaa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2avaexszk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oxnghsmi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dxbydxlg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bxdjqdef.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xfsrdrly.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rlonwuym.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nojtocoj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zwqibjzb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkcohk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2btflarpo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2srbkavrx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zzykxnqt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hhoxskev.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nnreiwox.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2knctetpw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ttkwxmci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oiptbvhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vcyeysqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azpwvgxv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwjjirpo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pbnelwjf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cisfzrxz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmxuaqev.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vcwgmnab.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gumtrffd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cemhfaja.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mkmdwddl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ecefsaqx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jalktgxe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ydoelrmc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kertjyng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2thxloyjh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jcgeygmi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dbowjuqk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ypluxhzc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jtpwgwvy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jzafgfys.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zkqayzdu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zuqtzsha.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2smyahzhf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2sxlwycrc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dufjqzgi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2imjjpgnq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qobwuqdu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pxlarihy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2etunosiz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nxlcudxa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvvzmlh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ridmudrk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jnzwvrfr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2scgzbpvz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2pwkefjwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2umuroyde.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jhfjouxv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iqjzwgww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbvjeys.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iwivnujn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wifojqwp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gxemfila.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vzspocwd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sofysvqu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dngkgrne.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jamqnyus.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xkvxxuck.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gvhdyusu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qxixbkni.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pezzrbsb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2grgdhbwl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jghocbbg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2awrpzxwu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xougdbzx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cbshzpzn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2quiucuxb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2enifxlxi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lcqubdms.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rmarljmr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zpfhwkuq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hfqjbign.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2avxruklb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rkvzioii.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2higigsxx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yadhkzaf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqkpeszj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bnhlfctm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fffolhqz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uoovqkeq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2runtnbob.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nvaeiocd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fjyxqskv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjaicevd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzoeuhqc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jebqwizo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2anirgber.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2grnzemxi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vtzuqgiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kunbflmx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2humtuzeq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aihpespc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nxgopqdd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ugaoggpe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xefyfnat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2itgiswms.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uibsmyic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uiarmvaz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yykknzkr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2shquundc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gniccgwr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mykzafcg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ygypsbwd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hqvtrmqr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nhtoswnx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhfvnxk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lqixipcq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bvnnciai.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bxpljdgo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngnslemi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qcsrinfs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yuuwticj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xcikqhxg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gsezgxon.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uvibdiyg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zyrccueg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gkienbov.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mzjkqjqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mryunyvu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2szlspbcj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzusomq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qxdatlch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wjrbccnx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pprfugsl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xaccuvof.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hlocrmel.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2iyzxcbgz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fvkpjgkm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xhdslxah.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2garyczoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pcsolxqe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tpfhtwje.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwioqugo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tonvjzmu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cwdmcpuc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xsskawiz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fdjmzobm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2csgwcsaf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iezadbyg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2svrsoqtv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gjpzfuwl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbcikpy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2raendgxb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xatjpgcl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ewmbjucn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2elybunjm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bkihfqtz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmebnasg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwrmbrmo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gtjznndr.html


<!-- 参考信息 -->