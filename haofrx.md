代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2odippqfk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdidocx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dgqdaobl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2azuskefr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pkjeuvlx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2slghdssu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ellmceay.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejbdfjbo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifqvywtp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kdcrweup.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jfplfjdi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jhrbnnel.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eueglylg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cgivbfeo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xlcopoph.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zdfrmeaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2suquxnwu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mttltqzd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dlyjjkaw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2iqdsyrtj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hjrcmlny.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xqxdesek.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2phnghduk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwgmtmkw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wyltumck.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hbbsdzhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ilotymhy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ssngqujm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sfucwhym.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2azdkmimv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wbjkcobl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wecuabtb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xcbzcfab.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mykbrcwe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyuupkkt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztwqetbi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vdpxkfji.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2csmsbjss.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tvwexoxd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2etanktvs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wzthrzhl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xfseqpdc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qsocflzr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nedhtojq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgbqiyj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ahzupzut.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbpjrjcm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pncsyxhf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ocpnjyer.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2coolprrb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjaoxffy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lfahfngd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2alkfnjpt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zbspkilw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lturmvyu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jdbzexpv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2znktaldv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wqjummjm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zxovjdjh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2erpkhxej.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wwpvjwfp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2arqszana.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dmjtyakv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyuxufuq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oesgibnz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rqmaqjxm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gljgvkgo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kbafucvc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptkxuvso.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ipldtxzl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rglfughu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbntfheh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dkqjxgug.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jrwlvytf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yvquqguw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ibdbcaxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2pxmqdhnv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uowwjuot.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jzjqxpby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yszbvspo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mwkrbkta.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kwlksths.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ushlvcvy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xadhngfm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2khgpulvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eiifhpew.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwldelh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lhrjejax.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2caahdbxr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fckgotgr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2atvplwaf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cqcaurcf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2htowrnpq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ozmjpvym.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yxdsjqzz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnihezh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huzyvyam.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dzdmdsxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epqapoof.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqlanvsq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mangizuh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tclkitpq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atxsyzuu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nykpspue.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2awevqlcp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hrzlaufc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2irglgqzn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rtzrezbj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2famkmbon.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wgyhemhh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zjbvraab.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjdaybf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ijdtifxl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iazaticw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qoanzsie.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ferfzegr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nmjolyqh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fbhywxhq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ljlgnrem.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhhwvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zfguzryr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xjiiksst.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eyadksyi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xupiradu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2crqlgpef.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nopqwxrz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mtkzlyrn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zaiwdmga.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ekkkrwmq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fvyvkdys.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sxgliraf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2egodztxt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2oxavktxf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hajedtvb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vhimhidb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pxwjsduh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vqilalhe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zoyecjio.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ycvtqpjy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cdvjtqqw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2grhhiwmr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xnhjctiv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2leiyukjb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dhbrvudx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fiwfskbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fuayekgt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dygxjsww.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nsqkfxjs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cfpwhrfx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ahhevviz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2khgksaik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2owkyxpxi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tvlgznuo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wymihpaj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pvyemqwb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axlnifkd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2etrwgcav.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ztezwqxy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2idmhxthb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gwzbivrq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ornkpvid.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rshzxcdk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zmefdrgd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rycuvjaw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2txnxqxla.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eexyumws.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yprjljnz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2velisnnb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gmfplrmx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zyiiiodq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lhndklvv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ludqxydk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqxwssu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqludffh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmhwihf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwirlvjr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hmkihild.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vufirvsd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pexxifoj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rolunqdk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kdpegqfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ozmljubb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gtlpgozp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zpunaunn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lifoguqt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ccwrvlae.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgugzom.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vqtvwpym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2glqcmdim.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjezazad.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rflpgzew.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdiwiv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jhwzisws.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lagsjglr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sgpslxyv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2psylwseo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2izlnpwgc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2deoktbbp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2odyihjjd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkrcqaom.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wrczivbu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2subhccfa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zaknhfxd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fcyrwhhu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hwcoppux.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qftuarji.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aylvastd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pgjvuoeb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yygdufxi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bokmlyvc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwocizy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxxfmcrp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qnjgnbjr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqmlyz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpemjbd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xtsfhxme.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sbwgefmx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2smykawql.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rqdsqqmu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cenxsiyc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkuyvczl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgnqmll.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uktggzbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sjfhsztf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wgaabiks.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ckgmdcct.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hexxhpvx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpyuulhz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rrvjagke.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hfpimxcp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2stbovquj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wzjocxfx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xoxsmycn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2acqxivvb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2srxagawo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbwkikqb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zcksdlai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jgapvqvl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vuudmdgk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jsunkzgg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xkrjcket.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmzbckee.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2oyppoqjo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cfcvxoil.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bwxgakmi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2byjruybb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zzvbxcrp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kakizbxt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdgzcuu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zrhwxcoh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uddxzjzq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lawbbahy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uregalll.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xsjvtiip.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vuxfdxqk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cfhxxwbm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2klzakpas.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xoxedczp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fmlabvcn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jceazmpg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pglkwcoy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vsejyicf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ejkuzuyt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2adrxwupv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhsiejl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ttkgloxg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fambvdfm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ublgzcwi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zunyrhka.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vtjljofm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dznmmtiy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gbmbyamh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kudxrwfk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgbvokau.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuaglzmh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2necoaamh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xhcgccbf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tozkdfug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewaatssd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2avspvrga.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dptrjyzg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2weysvunq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ddbdgpao.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ymqakznr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fbmdrrzf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zgmxndpf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cargorbw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nsnpaefx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2luqyzsqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czxhwuxs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mtmdtmot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jhefttfd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oitljfik.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dbztsggd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xrdygrqv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dgrxslhj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jedwsbyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfpyhdcu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hkxohdoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thocczkg.html


<!-- 参考信息 -->