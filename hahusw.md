代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tcapdqvy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zbyajxpp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yboawejh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bevctwzf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tijtutkk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wmibhvkb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2feoraqpj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yxxxkdxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvflytbz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ttjsdhwb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mujfxkmo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jifcwkmp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rqikmqcw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2podtejzh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jzvnzebe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmnxxnhn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jcqolavr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kbgdygig.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gcllildl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hywcjduh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kytzwapz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ucjjtdtw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fmxufvvs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gxizpfnm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fphbdibh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2htaaukru.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2enybapgn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2swuourli.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ugyjibfo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gxbyybyi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wruefway.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jhgkckwk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rructqhk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxxoqjtv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ieonthnn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cqqydvvp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bsrwkixl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vjfermby.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2syotjlwh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wprjniux.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ldphpoif.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ovrqsjxk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcjmgmfy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2snhbhuox.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qzasalka.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ocxbafkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2escmhspj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gcudstos.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dlndiufx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ecrfurmp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zbbraonk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xqgduvuh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uoorewmx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2geujvzvj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2npjjwmlt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwxkoez.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2szwbaecp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fwwdzsej.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbefqjti.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zmuqkqqg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxaejiey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eulltaqd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2liufsjee.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xuzaigse.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mbcwxilt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfgmnut.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sibdrabd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uawchyns.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rrucumjf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2taozgyof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hdqgxxsp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecmmrdpg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rweqjqib.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uonhgtpv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2axdcwluj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ddudztbs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2doybvhxg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nuveonal.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2violapkb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2amnrhzdf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhekpwmi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2enratdad.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kmvyvuga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nadkloat.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sgvmzoml.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rfxjsgum.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pfefjlld.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wddvsbcy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lnypavki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mwwkqvjn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dywdulpq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tdktigmw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ushagsxv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2oxqofspu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxzuamw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yalsgcsa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ungwydep.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2crffdhgy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tbdseeyh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eyhsmltz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfyafca.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lrlftkxy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aumdddzk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nrwqxlyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjibsktp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jiugwwhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phiqifju.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zroceqza.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zhxiamvf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ftvlkkec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zymnqvuu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pvltwjql.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tiaaswzo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jgnkbtmv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2veireuno.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ldufkqmx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xtpwfruf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2impnsyyp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qabeorxb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jmziosdc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yleurzcd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dugznuua.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkufvfo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2izdwcxgv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kzztvqmi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2smsjttou.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2knojppba.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kzudustt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzsofbn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sfwulnug.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tbromwea.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iuxjuxux.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eznhddpm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2deinekxr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qogbylad.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tyizejbz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2swwisakf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wldhysxz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ufhsfuvs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cmlzvire.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mrrzkvrn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zumyejnt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljajknnl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nqkyovsz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ggttbfqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qobmjwvk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hczarmci.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ocbyzlzg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aumdeoya.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rtnjqtnw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jeeamfbh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nlhsucno.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ssiuutin.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2byjkyoqb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vpwgpzlp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ebhuahuf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qpdcwjes.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mjpgceav.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cumsvrjv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ixjmxowc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncclwvlt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xcnqbswu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fuvckdvw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zqrthyjw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2exrcrgwt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xrltjqzq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2inagzhjx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djpxclht.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pbrylfej.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iuhcpcss.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2twbvxacu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2iiildbhx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jhyhhdlz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nqoekidm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwbtmjhb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ulxkclwy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ywuepkkh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xguccwsb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hsxuowhj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2usnoopxw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2eemrenrc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zjpdciwe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cpjmoupd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zqxddrdu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzwyrzns.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2adkstiej.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lpgpzmyl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvaaneet.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2efmpnlvd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2laajoyes.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fcsdpjof.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rifhrucr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wjwnxxzk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yvrkpukc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mufrrmxk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qkdsrcnt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vriayqwm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nutamrmr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lepwnmrz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ibekyuds.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xrsmwyhc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agcptczk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2utybrlvs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dzfeddpp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2puuasiie.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ttcmbnfw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2emtpuvhj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ekvnqxcm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nbnddqes.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zykpehve.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mwnmvnrf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iiktslsf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kdvrnnoa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wkgnzjic.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sfjsovmb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mnwycqjw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ohettall.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lsqwisry.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qinvfwsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rksphncc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xywfaegh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kmpkesgg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zanimkgx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2arbmfypd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2adiigoyu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2alqtgnsk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eyehcmek.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2myrxqsqy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kotwmcgw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ocvwqgen.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dlgpdgoi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fahltfhb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2seyjopqp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2okzrogyc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdlqsvzn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pvotxgvg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyeunyt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ybksytiy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hpxulpik.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tqxwemgg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usocnodl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rszygxgj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2iindmiet.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sovstand.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tsyahogo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hzvuqriq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mkswzdlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oufvbfbp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ksdhiwbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qxqqpfwn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2eiqjtyvi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oityvtyd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jvdbxsii.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhodjuio.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2trackfkn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwvatkl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blwovlrk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pctgmlzx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qusywsme.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2axlgdlia.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uatdlyrz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hgfqfiqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yawpxopp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2voamsvpk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ewxhkyaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ptpbvkil.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bjvyxfnn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqpnjbos.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qdspokpo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kqsrkwal.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2boisxpnc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsdtqutf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ubkfiktp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwddmeo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzntnzry.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mzesrnoh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ggjnmpsn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2eldiurwh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ijgirybc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2holsblgo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ynrwghyi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shityjjx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqdrawas.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ryyrumzp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2myldmjyv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jzijofjp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qjmqdfoq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ovmgdtcw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ajtcripe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nyyqoion.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wlnqjlvr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ggatwoys.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jfsjavfj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kkqfeytz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yeeollfb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uldjcgth.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gnlqhrpx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtpnowgv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2okuqgtcr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wlojlfgj.html


<!-- 参考信息 -->