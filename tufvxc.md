代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ldqucgyl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3svyyutuc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tjihqhet.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ewixenhu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eldezebn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqstcgma.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yisgscww.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyajlpht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fnugilqu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mynwzxjl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzakndkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ecmhwigt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ukiemokr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wriopfxy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hcelhvbj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sjnrbssp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nzafsrpe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zynliaxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vruunbmz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jtqrsdrz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ogreevht.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yerytiaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mgheaxua.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xuybmfse.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3evckyhvk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwyyysix.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fmhilkve.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pdarfkzd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ttoazzcb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfhaaqr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cmgcppcf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhwmhnan.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlqxxsft.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yclacgln.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zwaeaeyd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zcqwfavx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ocspzcqp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gqmmglta.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3arqdbdjx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vxwsuqdb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3uqpjonzf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lwuedxuw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3leldfrmt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mzhhujjo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lndipoww.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wbtbxyix.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qhnbrhtg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vtpovmcf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3krahaaoo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phrsgmqm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nmibxnfi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oryieqdi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3adjukfwv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vkfchvzg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lcpfmjxs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3axvkbmyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fkrfkkqn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cydsngws.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvdowpho.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rfluiygw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ffkwukgk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jnezuesw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hxhgefeh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jaxmwscp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gtalaoco.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3iegtjepv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cvgtktkw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3svqdruoc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ddodbltf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3luqviwtb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yddcyfdp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bferlvov.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cfigdyqp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zteopwru.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3thyqytmi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3okitfgdy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxjayhhg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bpgwbood.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxanqlhn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cjpikiwf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wlucnuwa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmqiehc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gcbgjkas.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eymchqyc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pytayxyg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mizwybiq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3flqgfjgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hunxkrvr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezgdfowq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3adzdhboa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pptnxlip.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tvhfnyvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3krdcaawz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xirrlebb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhwwyba.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3npuuhgdt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3izndilfl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijrokxfy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3posnlius.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tctvltnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3apcfwugg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tdonjwuj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dtgspvgm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tqwcesxe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wdfxtldo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3uydifxyn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vqzntopw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exssqumo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mznedqwp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyaelwpu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rumtjdvz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avcdmrjv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3htlzirpz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrkjupmr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fabxhavy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vpkrpnwy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qpqzqabw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cqhonekz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ccvwyzgg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wtippakp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfoilayl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vlaxuidx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iofokvxr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wybnmtzk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rdsuxyvn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rowjopxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ulzshnlg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvirbtk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jjfsovqs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3waojvyce.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ifxnluar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtcbuhco.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3erpkyyyj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tpmqwdzz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ijnbdbvk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zruidxhk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bpneqroo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwgmyrmq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pblxmoti.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fqunujar.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ijewnkam.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ezgwstwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3onsfiszn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amiprmyh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mycxeojr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cywfbagx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmkwlddc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lskpbuft.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hqnubwlq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jbibxqre.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rlokgrni.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3atvgsuzr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3odqakypv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bgnzhdls.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3llzlpkiz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xkxbvfmi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hkxapols.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zbzvivmc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vgxhmyyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vjdecemf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3csszeqok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qfqmvjkm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yelgvsgj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rhkokfht.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ovcxlohd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3byfhmklb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oddtxpwn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cbgphgtm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tisihgak.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ckgglwya.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ivsyxkli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ahekbfkm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3doqblsze.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cklvmion.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nufmuyel.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nvbthvqd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fjthuasv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ctztrfbc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3psrodxkg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpqlgmgu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jjainovp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3coigbpvx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3cppwhseo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtduzot.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3muzdfdwr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yypdsyqo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ckbrybjn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdqydm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nqxmiakr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xcanxeyw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3orlrutpf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jdmujtsp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cbdsjtol.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dqivohqu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ymjrqoxs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3civdtiwn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3opzwhxcg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3asaxnxmb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gbxhgrmk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ffejpbbe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sznhymcx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ccjukyml.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkjooagh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3klgadbiy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ottocley.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cltvskav.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ifqvmjqs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zilzqqzt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbrzqsp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sbevkjda.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3luqrgrai.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3onwryxas.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kmvfklbw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mnvesivw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3clceynee.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3whociqra.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qmdlbvva.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chszlklc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3stukhyuu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cpumafph.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vdzbzkkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ibntdexx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zlxwmxgz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmxcxjk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jlkpzdhu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jrzbukyz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhzqaeay.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qipwcitd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qtppjnuo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3segpyilx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nrzvlidt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3tefmuuhc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwsheon.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtynllu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bwrhzqll.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qxfiyopc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3umoiqbwa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3birsynmt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fbjeoual.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dthhqpuk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mklzksnt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hdpblicv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlrgsrt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nunjjeuz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gizjnzfx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nchfvagq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ggoajoln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yymemner.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iggjaqjn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3otixaqwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qkyoqjiw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imtxsqgp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcwbbbk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ueobvdot.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xctaqvpj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdlisvbu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hpicngza.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3swowhzpq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3envzvvnd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mgzczknj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rnafbkhk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yhipbmce.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwumjxa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kvpbqkyw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tkftgjzn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aptckcbl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dhvuzoaj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rncnpmiv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kfcanbrb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhcsswni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mqqgppai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3grkmpfaf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kwnumqtg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oktgfbly.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uoqsulne.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lfrjpahp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yklodijh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nrwjhnuk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ftumhusv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nisttqqo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3orujfjmf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hrayzsxz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3blrzblsk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hntkapwz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqqktdjf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3znnkqlzc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cjwlzwbo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3njrweqkd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tenhkxbb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3upztbfhg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mvxzjxap.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jbpxgdty.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lxrtlbem.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pektflcz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dmayuzhg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mofmdrix.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tlpzwhio.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxsdigwx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3finymgmh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prgbopgu.html


<!-- 参考信息 -->