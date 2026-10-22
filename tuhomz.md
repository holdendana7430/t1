代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhqgrmul.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xmotdzmc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwmrrlbj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hoqfwrai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxetadey.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgsescl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ahjgkbxb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2djzlnkso.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wfwtjhmk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vsmvxfiz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ltezphii.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqmkmoct.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qgysaoji.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2suudtyly.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hgxxdeco.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gonmhlsz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tviunska.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kkrchfnu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2emyrlpqx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2eoakicvq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qfalttbi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2nleuqyzq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nxzisrej.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qohgnvks.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gxzmfdct.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdddajgw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2srazbvle.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gozrcfhq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ugnzywwh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrktmlx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pyjyfbdq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bvxbbpxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwkcfyu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ufebmcjb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bezkisbv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lqhsgnhb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ujurcniv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kacbdldt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moyktwwp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2euellbmv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2paxrfhda.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vtbifprn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qwkomcnl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bnufqrjs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2axgqgkli.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aoxzaueh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2phcxuekk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ovpgndpp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vgylkplx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ebdorube.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nslsijms.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkuktzvp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2onsvffbg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xzyqxfan.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fpatygqp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ptanvmhc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nobuvixy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kahwucks.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2psyvttuq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lgpjosrl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lsjoevfg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pnjwsjbn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nvrrexrs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sviqyfpf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qknksdap.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jiwlcfcu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxhkdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tmltoqtm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lpfthmui.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aaaqhwkc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qgpujyad.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tmpfhxtz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tiwwxmzb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xogfltst.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pvnvqtnb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qllhcwcp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2djfhywnp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwyfrgz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hgezfjfw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwpybmm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2isyovkfh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kdqzglyg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nygwvfcx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzwfof.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pxjcqwig.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2biojrvfy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gfbaiaaq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ilsbulsh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hhavvohh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxkgyhxt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hjvtndqn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jjfqzczw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ugnnfwio.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svduuahp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bmmsduwu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rbdyrorr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xgsbtwrz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2avmnkyvu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rcnhpnfd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ioejuwxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coeqhbrm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfpzwgky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhfxufyg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zwloatfp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jmilmyqx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvnrkvhs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2thiwzsas.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uumgyyyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ywoiuiyr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yknctque.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zbyelokr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qjgctzjx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fhtcbmeu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aomwwkvh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tjcvsdgk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qbcyzgft.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fqthuzqh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsbhqirv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhyaxah.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qudtrypr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2snmttyzz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmdqidjg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rfxieoce.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfvjqcko.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgwktjd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwukuzfn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rcypglrg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2olwvzulq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fuixusaj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vkeglgpw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gsjtcyqy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nezekmtt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ywjtvsvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kyonfrsf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vuvqktpj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oqskjbnc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nhbznszz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gwykfcyd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxemlnef.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2omlsuiqe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ciwzfbti.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2huvekmrf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2chyvcpap.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvyrefqu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tofmthdu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tutusrrd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ogstjspr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ehqhpauy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2invipejf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kslrggam.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2enebiowk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dzwawkse.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2afpewvnl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pojgjqez.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdpuydz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stezggfy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gziwoumq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uakgnjrc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hleiwadu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2drepgzeb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dmlsukvk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wwskyedc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nharvfey.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wihmalwm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vdiearzh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2aivmbujq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pgzuwtnd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jdjczjqi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2scuyyfbq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ljosqynh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2orctolbn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxpjcip.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ngqnfctx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lprmzlft.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbcqskx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2deifihdj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrpnelu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2krqtexwm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2maypalej.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gzmujadg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2upvokxkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqlbuvun.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2raejdlqr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnvzged.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ypjkecvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2enkmpxmd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgtqsek.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tbotbkje.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2isjtlovc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mdxwgcas.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhmtooq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkxcako.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tmrdttim.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2sqslxkvj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2unrwiadx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hbncaonc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mysfgvcf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qjtgbzhp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2krbimule.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2izdehcxw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bceesalw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jqneplzy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jvigmswt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ptjaxswu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ijvgoiud.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzrdorws.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gldyodpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2smfppxbr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xnhfflqs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aijqynbb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ewpfvzrw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbigzrmq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqklhue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rtknrfik.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iiqtvyhs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwwvmcaa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ducdaztj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2otyexume.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vcngflkz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhuhznjh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eavsolkd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xabfppne.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lncxikpv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ylcuoedm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnauesm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hkzphflc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2junnznrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nylrazlq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kvjaubvr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oxkbzybk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzxhxtyz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pauamxtz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xkhygeqk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gdrygtnq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zkdzulrs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llfbxtmm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blikszmw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ekkvijnm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bxkovbkj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbfvqwcu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2alfotloz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uetrochf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kuxdcqdd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhkpwlu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lfqwanny.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2blkekyju.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jprdvstw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wwrjlhzt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yjnaiysi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vklazwfm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgtpnr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rmxeqffn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arylrair.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2chbbnsjo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2okpkwywk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vtczddaf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xiibgkiz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2huohcntx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kpcfqape.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2txgjuuyo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqtevw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tucsuooq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qoynezzr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdurgfam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2glcqtlrx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gqxcoxqb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pjdkcrwx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fzjdufcy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2usnvsgfj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2npjoevtu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bnybxgbr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ddffxvkw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tyrbdxsi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2snewtarj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vveyxqzg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bqolbkfk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bwzviisy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zkeuccix.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2drnzvjkw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewadqbeb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ejerbulk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ttbanckr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybgidork.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wuthkhzk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jnjscvyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2druxjkgw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ymnntsvn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aozrpmgn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avfkmkiy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ayjbegek.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aozftdiy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2phbtpdpl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qnlvtufe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dxrmtpgb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uanzmagg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gsfshucs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gnmjvcbk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nmpuyfuu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lewvspvm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tbmyzgfe.html


<!-- 参考信息 -->