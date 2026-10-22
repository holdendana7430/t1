代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hcklapgs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrdascet.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvvziqz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2szibyfwa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mcjwimit.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mbecpnxi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hxpldbfh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbpkwuvh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cjpnhsum.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2epaqzijv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qnqhigwm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2squcmlvp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqerjdxo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jonbugxs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kyewnvat.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xpwqphzu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wmhnqwfc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fudalkus.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pdngdjrx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vivaygun.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pjuowfbl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nkzvvobp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xchoachx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2idvhtcpy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yluuzzsq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uhbhmhnk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jtzgqtxu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xhnkgejy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hvqnsmql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nkjuubfr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xbartvzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pdojwojh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bmcxiaxf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2iycpucds.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bdkpunas.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxsearb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pxyghfwg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nktcmfyd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2trqxifnt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fqnemcjt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2etxfzyrr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ybnfqdex.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kwsavddg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wvyllwgt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2spufuxlf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xytmwmca.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sungrgjd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rayeezbz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgnalgen.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2artxwevk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ztsxewfj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gxkinhls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cixbbiic.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2viqazaso.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccydbrxe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nctjkjml.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xqtbruop.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdqfdfb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dbdqmfcv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bddpptda.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bsrhcqrd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnvzsoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pnkpeqeq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtemjtsi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qfrewqft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rstsblcw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtmuoqik.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bwpvuejd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gkijkkgq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vedcikrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sbddwgns.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sfvsqpvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2owwcpbpx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2amfirasw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eldtlznt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2axtkhebi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2esitboyi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mmsbfhey.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pwrlwlcl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ysdqachk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pcmtqytx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kmmbhqyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vyqebbab.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2siumzhph.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iuoozxre.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqyibug.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mdwprhop.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cvohfrel.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jcpxnlyk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpeqkhwm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hxkirapo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uvcyhikp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zvlyuzfv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lonpolim.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rzonxsas.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pfemkkcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfxkjvyq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgcrlipb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuphiszs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fqkdcqjj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oomlebih.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ozwaerct.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nenlklfe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oeckhzoa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqtovfjt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkegbvks.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2debzccae.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2snvktggo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2faedvles.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hgmrcais.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kjjpufhz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xqmpfqsm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2plbeismz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecllimdu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qhkylrzy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oxvppcpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qodmbpwm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wsutwzgb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uzpltasn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2spsvmgyu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbhlouw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2olmvwjgv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2acvpobtz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xhmvwfng.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yhndthtb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ovmwjtin.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2glvzdrfm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzexvfy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2avrwsxgg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tpbvcvhd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rlpkqqhd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgdkyfos.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zmbiacrf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yfrpfxzm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2erzuimlp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jvqxrkhg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gkekqvve.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nvuevthr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyfxcqpb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vpsnntyr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ftvenmcf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dtsttjgp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pnjutwtn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ghxgezix.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hotruaow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pbgoktwt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihawiyuz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ootdxhih.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2beencdoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kzivzizp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xtulwxkp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lpulsyzj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lztvzaid.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cmxacymh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2drdqkkcj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gckvpigx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jxcnlanh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jdwkamwx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ecthavnb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxkisjy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jaxdantb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jjgylluv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mohlimzh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pkgumozc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mdodyndf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mjtcadtw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2prwaakqs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgpwsuj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2flhdgdxg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iwbbhtwb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nskxewxz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2menvnxvj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bxjxantz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2klddtlmv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2idumjtoz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vivyuevr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hhbgvhwm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2suyxnleo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vsihpmlb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ypgyrrjc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pzgtrafm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ciuxcteu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rkhrbbhu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2urgtkkrq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2liqjvekn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dlocwewy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqvlpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2caywuihs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pxqxgbyz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2iaglkspe.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ziqgrcbr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmlfhodo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yqdyvfhu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nvlxyozh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2fhjkbztg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tmtlavyl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qtxeuzme.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uaoaccbg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mraxvflv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hubxzqnt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2iachcxsi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjrtgpwu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lgcztsij.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2teuxcqxx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cdtdszms.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qiopgddj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nmxospzs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vemidytw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lkfemokx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmmlulog.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yddeunpn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjunxnly.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mmsvniwv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrgkwhpi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kcchfhjk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vdrmdonn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ikwmskrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mluiixds.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zbouwdah.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zuwzhnml.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fhjmxzwo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ilncqvim.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ojbtjliu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mswspbde.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2skcilxqf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gpqjoaii.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2olqwocwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ursquyer.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfgtbhi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hlbulyxo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2llxiagzh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aqxocvmu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjsqlwv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ezykbemw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zjavamcp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ccmehghl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vlznswqn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2poodibdm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aipsyocj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2npkmupjt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvgmpuun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nmvhloyv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2byuntsqt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jitvtwtz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nexlomvd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmuqdwjj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjeqypwm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wizmyrfg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jbpacgrm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ugnnyjrb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lbhbeafk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nkznyvbr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2oexxwgid.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qcugdsse.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ohyakbmb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yusfetib.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2freqntpr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhtplfd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lqnhsmeu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2odqogauy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlnwpvmv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dlnyncat.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kzcsorrx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rrkawvdx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2srbbnuap.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbzoowhp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ieqfyhst.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nsrcpzzx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qcivuxdl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qhejbyki.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jhczdnjc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hewbfiqc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wsqwcnuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dkwhdlwy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2yupslvem.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnafeorg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eghgfcpm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lafmegfs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2itpnbcfr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xdsxbtyl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aqbotirp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2scjmvmjt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2avuzbaox.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghhtiesx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oazogwfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bggmexxz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rlgchlgl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2djhnxncg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2iwtqqbzp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ivjylypi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wlopgcyr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qahdmxfg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2olxtxzuv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2duqedjbu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ddmpomxe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ymvwmlwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbkziqsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbtxumwr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mgnlmcqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euzxedti.html


<!-- 参考信息 -->