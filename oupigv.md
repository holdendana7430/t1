代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fkwgyand.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vnqiaufg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ycegvnqu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dhhttfic.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xctbqdih.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qcykjwsk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lvaacphg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nwmcmrbe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eovcqdyd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nxpjtsvk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lvkucdtv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uybagsqo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lmoepagg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lnhbnstw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xthlpnno.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cthvwxlz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pjghqieh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xuqfbbbf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2shqtcuit.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2shggmrmb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxhbcfti.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bdwaepla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2capuraie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zawxazmx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jamnyhbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gokfspki.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xpgvnzik.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ojkfawxu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gsaxcvub.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2sjqzjpvn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gpsupnmz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxqiqsr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdynsss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjswgvm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syyexpzj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uflmynut.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzkjtpx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ymucksbt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dztdvhfi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nobehlmx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2nkykivgr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2uxzpjyny.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jeazqjxk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2twdgqvrj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ukrxdbrr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eziyzepl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ouownqsc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ismctdtb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2aggtlfhy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2huytghwm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vlaeklto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2falhjtoe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aqrvilqp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kkzbxjhw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2curmqqsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oypikhsw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zlmmryxw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uhgmtazv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxrrgnr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwqnzwyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tybtgqkl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hubbuuzn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yhmarcfb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wxeyldlf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rsoahlsd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xhmplidi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2biaulhtf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qmdfjirg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nofacpln.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2twvcvhdt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wievoran.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtxuqoqh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdgtxjd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sirgbnfv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2juoujdix.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sdnwgguu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwwgabgy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2uipxkzgq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juyozpcd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nycmhtmh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rhyfrhad.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwmmtmp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zunvvlbl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lkqxyeqj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dxtbzatt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgvcjojc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2etpxykmu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hnjhaqji.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2laordzig.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ecdusysm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qighurpc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gzyijgjj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nbfglotg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gwthsses.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oawjkkay.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvfnlmvq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2umrpbeta.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2srsiyehs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mmlzgmtc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oomzapyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aoyaitex.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kuxtithq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vcedbquv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2amgrmttw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ebrmteru.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnbnsda.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yvlgglth.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mwnadqsv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pqzfwsan.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vqbpzzrz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lysrnumv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kudhrvup.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2skbxrxtl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhbusaiy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vpvtrowu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lygkxqmy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hofcxpfi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mkpqazxm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eshtwrpo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uecakzkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnksrxco.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2adknltot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpmxehpv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zakzdxsz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xytsrugf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cbnsahxl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2usmjrrbp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ytzghfwg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zpqaczne.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2huaeidpr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2duasqmwg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oxjrjbeh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujwovetl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vzaauzmi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dbnatmhe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxaselfb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kkedlabe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ouugheps.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yogqvzfn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pcmltzym.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wcvyessc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wnkczqkx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zezaigza.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nlorbskg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bnirzkzz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2koqdrhpd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hskupfrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kbjltopd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vbszpeky.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tpwgmhur.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jsytyesa.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fgykxqws.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vtajizqm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dajyuhpr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bphxonna.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwpeuppc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vfmizkwm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pobxqiki.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zeftrxoq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vyyqpcot.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vlkptcbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jnamaphf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2erlxszhx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2diesflds.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2atskwtuu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jzlhvyqv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cjfyqtlx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jlfozpwe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2nnzgdkib.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pqizwaae.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvoutihr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vuihdaxd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gfsrrkmr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2odpsdsbw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vodxekjm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmacmtiq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tuzwtcff.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tvunfwxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2molipicu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fmoseafm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vohxfufn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxwqpws.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jukyrqzj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2purrozhi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qhfinjaa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dioiydtt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2blgzbitc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrmlszp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nkllhxwd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qslldfmp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xkksfeaf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oitmlvrr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2divhbndf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjwadh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qqieyudt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2givxcftj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2igodokmw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqcwnlhh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ydkimcpy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rhfkxaka.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uopwbltk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2apmaepkx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gyevixkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzrypsmo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wnhqotxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rimpeayd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sawkuvuu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yviouzhs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lxnjdhno.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tngovtzf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jyvvhhki.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wznxxhih.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nrzywcvj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yfvtdxja.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijbngpyw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cbimaooj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vybfsfxx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kyvvssww.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nayeopct.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cqrmgjfk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sikjbluq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2miwmrdqs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hjjqzhnz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2goieioej.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dlsknbnb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dvrqltmm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcbgogtt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qevrwdif.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2putboxoo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gdzvbnzs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2oodxhfxd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zypepnku.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ueawtdqi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2uczlnhqm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hxtnylpj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mydqkmop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qscbrdgq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kvrehqfk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xjcuiiob.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lblvadyx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2efdrbfsk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dyzaychm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rlyfyfdd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxtclhi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tussvtni.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gnvdrbkg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mcfxnmxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpbevthc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2btjynckr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2saksxhoi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vuepfins.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tcajelkz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2niqhbwvu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2odcjbcqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2djxgwcqf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vkvldbuo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddasejqe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ilupeleb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vwjtbabe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvrhxm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2thyhbgqf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2djywltaj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2phpmcwjr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qhjdacvl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xybexsws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uxztuazh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ehseynmu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2htnelprt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fljnwghr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tdlzaial.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pldufjou.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsnbveq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2alfhgziw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ohazaxox.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dgfinimc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ixsllzhm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mjginzla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2isvqkxpg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2juduialz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2caogmbga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uczxksyt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vbzlbxhe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nihepcco.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hxzkicyw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sayuwvzx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jjgnqcim.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fdtkrrnq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjszcveb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sextpguv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbikwdhm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvtuscpb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zfcaoshx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xxjsawdk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jyzxuqgc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gknsrofz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oazvinpa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lirpjwkj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qkovymgg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oyiebbjn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apszjqsl.html


<!-- 参考信息 -->