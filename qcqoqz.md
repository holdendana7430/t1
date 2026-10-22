代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdunrlj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2efwarkvm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fwtlydpq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xbxyzhoe.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lffykijg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qiztzmil.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rwmlvyos.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2aamsschk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ejtjnuws.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jpuclsdh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qvctslha.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fdyxvtis.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lxvrzgbz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2izdymrru.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbtiwpde.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pyqyedea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mjynbodx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tlirlypy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2clfpshxf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tewehequ.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzojfyyf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bwsnwywu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmusfeuf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2odbfjrbt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wsrjnfmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lwidffpn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfmevssr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2suunpvlg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qmohujxf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oubzhzow.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uqikftzl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qoqjcwqv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cynnserb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2asfgpfzf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddamblnr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2imziffwf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pugrvmum.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhglvvx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pvcbrzrv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2omexlxnp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tuojtafz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jyuuwllf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jimiomwf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fihvvjyd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2czcogovm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgtnxoc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tcebmwvd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2stfxxbfc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjktfpic.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tkiugxcf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rypwqozp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jxtzkvbx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iwxovxbh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qoasyxbp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2inhbvwuq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2stkerdfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gnhqgndy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2epiqkzji.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xiynygcj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ttefxsvi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jydkwcso.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uhvgwpir.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2amcepqaj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bcdnpiro.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2llckkumz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wzgrfgfj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xmhaljia.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qywwzonh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2azuzkaur.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uxxwayoj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2siqnhcam.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uwxrucwj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qknwrgdv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qoqxrjnm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bszozowb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jihguuqk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pyomjfab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cscqemzu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2apqxfgxb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ftnzmxvx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lvtntxpu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jefxinbr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dnvcqygc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uggbpgqy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kkxykeuq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bkohhqss.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ajgzgdpi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hmxhhgsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2biiafdmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2udywyjrn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlwkuhur.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vyfwqwcc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pdlhbsah.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2liqsvzlh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tbxjsohf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tpjjihhq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qicmvzsj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2livkotrc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2awulmybx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdafxuw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qkdjbbpv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jaddflqf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cystlecr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gomigwxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pfrplfor.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cjqigkmg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcdipcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfknwqvs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxyrwpbd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ezcgxxzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2upgmnphu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xmzowyuj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2htprjrvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xnkwdndb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uydweoka.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2urjfekyl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2htctzpyb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkpsxeut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bpdszdcg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xvulqvrk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rrbaebro.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbedtp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqaparx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omtkizot.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lmllgjjl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pksyarck.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zelnekdg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2venltgab.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yvzeymfd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vyuduaqq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pqocqdwq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pifpejym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pudcufvf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2focbgedi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaeprawg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kghgdhsr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ceboamva.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pefffixm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pupisggd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qislotfs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vcyvxeqr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ojjattie.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lcvfkaaa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mhyajxsk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ekxifnkf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tflbdcyd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kskhdgpz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mktgdixk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxtdntd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ynzufiat.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ralugerq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2syfjukoo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dbpguxtx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rlparhie.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lugplmxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hbylcuwx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbrdmve.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qenwbvpe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lprhozcu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ifjzxrhi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dyjifwen.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekehsext.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zlvjyjtn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mbjqhmni.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xnqhtzkr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jpapkrka.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2prcalzgr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zeizlnrg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hlxbmnbt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2prepscar.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kndtnygo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jtwzytsr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iofyiisa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kotpntfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lrwlezzw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kohaswwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jcspifvr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ryirmmjq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rybneigo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqotuokm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xqpaefyl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gppsjzif.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbpywyev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gehdgjem.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cctjlxeu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qosbcxfi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cblfjkbm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hjzvisje.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mxxmnrru.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cgxgiiiz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bkfldqaj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xmogcfdo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xntpwlgo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gmlvrhud.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2efuwgnui.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqhquyh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ffafrgng.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vcfqikkz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vptkyfig.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xjbkboky.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qnxbtqqd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qqhistof.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lxbrdcmm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2socfjuls.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ekkpbynw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2krlcrivn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yjodwsqh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cyymaywz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nzyijnsa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eyrpemjq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nihidpns.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nonwzfhu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qxoruzlq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2awngpxop.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2sqpiyijt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tovhwrjo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2syclpoua.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tczqjznj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2owlajtyo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vmrzvyoj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ajywtgem.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ukblijde.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2skmvbrbw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbsnfrf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tcaghosz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pwegkojp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jjfbjskn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssdfteja.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zghkmbgc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xadfdswe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwdswvxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rvvasdjr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2elgkqfik.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fikbciqo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rmccaufb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dlmzzsis.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ibjmrhsq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yixpqugt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyhswpgx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rkiyvekm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mttbdmdf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2isqcpycc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ermfrkmt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vxcpuksc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ybldxsrs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrqjhvrv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iijxlnyx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rathtchj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlfppvqe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kiddcztz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ygpoafar.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ktpebgsi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2foywqkjx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cktyhlxa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtdwdyia.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kcbnulch.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rhnthylu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oqarpnsn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2prbeavat.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2osdyizqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbqbetc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ziyzdohk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbiznjnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlusqjwa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkenuid.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ozevsqcb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2malguttp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dbpeqooe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xholhgww.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrrxxff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ohtvpvmd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oqiaveyv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2iajvuliv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2etjfmder.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dckpegza.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zpuxsply.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jpjwsctb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2maehqcgk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2aaxkjzjt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fvxqvpbp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tqtusntb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ymmyairl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkjxbgf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eycztpay.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxrcwsfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2eccvbbol.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wsfwfkty.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vokjtyqp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2robwmzvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cypjqesb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kmvwumbk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2obysqznw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rcrkrcqj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aicdnwpw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qokcksui.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyazbfqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lwfxyumu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2offlbgcf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ktrbfadu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oifpnjsa.html


<!-- 参考信息 -->